Fisher矩阵

贝叶斯方法
已知对于宇宙的观测数据$\mathcal{D}$，以及对于这些数据的解释（模型）$\mathcal{H}$。我们为了确定这些模型的可信度，即模型对观测数据的符合程度。这种可信度称为后验概率，记为$\mathcal{P}(H|D)$，可以用贝叶斯定理获得
$$\mathcal{P}(H|D)=\frac{\mathcal{P}(D|H)\mathcal{P}(H)}{\mathcal{P}(D)}$$
其中$\mathcal{P}(D|H)$是似然函数，$\mathcal{P}(H)$是先验概率，$\mathcal{P}(D)$是全概率用于归一化。
在实际问题中，可以进行简化，全概率$\mathcal{P}(D)=1$（因为观测的数据是一个确定的结果），比较不同模型时先验概率$\mathcal{P}(H)$也是一样的，取为一个常数。这样后验概率正比于似然函数，具有最大似然函数值的模型称为最优拟合模型。
根据中心极限定律，似然函数可以用多元高斯积分很好的近似
$$\mathcal{L}=\frac{1}{(2\pi)^{\frac{n}{2}}|\det C|}\exp \left[ -\frac{1}{2}\sum_{ij}(D-y)_{i}C_{ij}^{-1}(D-y)_j\right]$$
其中$D_i$势能实际观测值，$n$是数据个数，$y_i$是模型计算出的理论值，$C_{ij}=\langle(D_i-y_i)(D_j-y_j)\rangle$是协方差矩阵。
若各个观测数据相互独立，则协方差矩阵成为对角阵，对角线上的元素是各个数据的方差$\sigma_i^2$，从而
$$\mathcal{L}=\frac{1}{(2\pi)^{\frac{n}{2}}|\det C|}\exp \left[ -\frac{1}{2}\sum_{i}\frac{(D-y)_{i}}{\sigma_i^2}\right]$$
记其中
$$\chi^2\equiv \sum_i\frac{(D-y)_{i}}{\sigma_i^2}$$
从而似然函数变为
$$\mathcal{L}=\frac{1}{(2\pi)^{\frac{n}{2}}|\det C|}\exp \left[ -\frac{1}{2}\chi^2\right]$$
无论是SN Ia还是BAO、CMB其参数限制的参数简并方向都是不同的，它们单独对参数的限制并不强，因此需要进行联合的参数限制。我们可以定义总的观测函数
$$\chi^2_\rm{tot}=\chi^2_\rm{SN}+\chi^2_\rm{BAO}+\chi^2_\rm{CMB}$$
于是可以获得联合后验概率密度分布
$$\mathcal{P}(\theta|D)=\mathcal{L}(D_\rm{SN}|\theta)\times\mathcal{L}(D_\rm{BAO}|\theta)\times\mathcal{L}(D_\rm{CMB}|\theta)\times\pi(\theta)$$
其中$D$表示数据。$\theta$表示模型的参数，也是我们所要限制的。

MCMC采样原理
在参数空间中选取一个点作为起始点，并通过多次迭代到达最佳拟合点的位置，在这段时间内的采样不能真实的表示目标分布函数；
还需要进行进一步的迭代来使所生成的参数进入平衡状态，并且把一开始的采样删掉从而提高采样的质量称为burn-in过程。

宇宙学中常用工具：
采样工具：CosmoMC和在其基础上开发的Cobaya
理论计算工具：**CAMB** 和 **CLASS** 两种独立的Boltzmann求解器，用于计算宇宙学模型的理论预言，特别是CMB功率谱、物质功率谱和其他相关宇宙学量。不同模型需要修改其中代码。
似然函数计算工具：**Clik** 是一个专门用于处理CMB数据，可以将理论值输入传递给似然函数，理论值和实际值比较，计算出似然。


MC采样的流程
1. 在参数空间中选取一组参数$\{\theta_1\}$，下标表示步数，同时计算似然函数$\mathcal{L_1}$。
2. 选定某一步长矩阵，得到参数空间的下一个点$\{ \theta_2 \}$，并计算似然函数$\mathcal{L_2}$
3. 计算$\mathcal{L_1}/\mathcal{L_2}$，如果大于等于1则接收$\{\theta_2\}$作为MCMC链上的新的一点，然后再次进入步骤2进行之后的迭代。
   若小于1则先生成一个在1-2之间的随机数$x$，若$\mathcal{L_1}/\mathcal{L_2}\geq x$则也接收$\{\theta_2\}$作为链上的新的一点进入步骤2。反之则舍弃，保持$\{\theta_1\}$不变，进入步骤2。
   (说白了是按照$\mathcal{L_1}/\mathcal{L_2}$的结果作为概率是否采纳或拒绝)
4. 使用多个跑者（walker）同时运行，当收敛判据满足并且链上有足够多的点时，停止运行得出结果。

关于收敛判据（需要推导）

关于步长矩阵
我们常用高斯建议矩阵。
高斯型建议矩阵指在参数空间中使用高斯分布来生成新的候选参数。假设当前的参数值为 $\theta_t$，那么下一个候选参数 $\theta_{t+1}$ 可以从以下高斯分布中抽取： 
$$ \theta' \sim \mathcal{N}(\theta_t, \Sigma) $$
其中$\Sigma$是协方差矩阵决定了候选参数 $\theta_{t+1}$相对于当前参数 $\theta_{t}$的偏离程度。
协方差矩阵有对角矩阵和非对角矩阵之分
关于协方差矩阵[网站](http://saili.science/covariance/#:~:text=%E5%9C%A8%E7%BB%9F%E8%AE%A1%E5%AD%A6%E4%B8%8E%E6%A6%82%E7%8E%87%E8%AE%BA%E4%B8%AD%EF%BC%8C%E5%8D%8F%E6%96%B9%E5%B7%AE%E7%9F%A9%E9%98%B5%EF%BC%88%E4%B9%9F%E7%A7%B0%E7%A6%BB%E5%B7%AE%E7%9F%A9%E9%98%B5%E3%80%81%E6%96%B9%E5%B7%AE-%E5%8D%8F%E6%96%B9%E5%B7%AE%E7%9F%A9%E9%98%B5%EF%BC%89%E6%98%AF%E4%B8%80%E4%B8%AA%E7%9F%A9%E9%98%B5%EF%BC%8C%E5%85%B6%20i%2C%20j%20%E4%BD%8D%E7%BD%AE%E7%9A%84%E5%85%83%E7%B4%A0%E6%98%AF%E7%AC%AC,i%20%E4%B8%AA%E4%B8%8E%E7%AC%AC%20j%20%E4%B8%AA%E9%9A%8F%E6%9C%BA%E5%90%91%E9%87%8F%EF%BC%88%E5%8D%B3%E9%9A%8F%E6%9C%BA%E5%8F%98%E9%87%8F%E6%9E%84%E6%88%90%E7%9A%84%E5%90%91%E9%87%8F%EF%BC%89%E4%B9%8B%E9%97%B4%E7%9A%84%E5%8D%8F%E6%96%B9%E5%B7%AE%E3%80%82)
$$
\sum_{ij}=\text{Cov}(X_i,X_j)=E[(X_i-\mu_i)(X_j-\mu_j)]
$$
对角元素为$X_i$的方差$\sum_{ij}=\text{Var}(X_i)$
非对角元素为$X_i$和$X_j$之间的线性相关性


模型选择判据
参数比较多的模型由于可以更加灵活的选择参数取值，往往$\chi^2_{\min}$更小，$\mathcal{L}_{\max}$更大趋近于1，从而使得最小$\chi^2$法倾向于参数多的模型，导致模型比较失真。因此需要一种惩罚机制对于参数数据量大的模型进行惩罚。有以下两种方法
Akaike information criterion AIC判据
Bayesian information criterion BIC判据
$$\begin{align}
&AIC=-2\ln{\mathcal{L}_\max}+2k \\
&BIC=-2\ln{\mathcal{L_\max}}+k \ln N
\end{align}
$$
其中$k$是模型中参数的个数，$N$是数据点的个数

FoM明天看

贝叶斯判据
$$
BE=\int \mathcal{L}(D|\theta，H)p(\theta|H)d \theta
$$
同时考虑了参数的数目和数据点的数目，也考虑了参数空间的形状和先验假设。


