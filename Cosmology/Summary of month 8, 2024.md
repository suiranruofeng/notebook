# 1. 全息理论和全息暗能量
Hawking提出黑洞的熵和其表面积成正比
$$S_{BH}=\frac{A}{4G} \sim L^2 M_p^2$$
系统的热能E和熵S和温度与尺度成正比
$$
M \sim L^3T^4, S \sim L^3T^3
$$
L是系统的长度尺度，紫外截断$\Lambda$

Cohen等根据全息原理论证：
紫外截断
考虑最大的熵不超过同尺寸霍金熵，一个尺度为$L$的盒子，其紫外截断为$\Lambda$那么其格点的尺度为$\Lambda^{-1}$，其根据有效量子场论，熵为$S \sim L^3 \Lambda^3$。考虑最大的熵为黑洞的熵$S_{BH} \sim L^2 M_p^2$（这就是上面的贝肯斯坦霍金熵）那么有$L^3 \Lambda^3 \lesssim L^2M_p^2$，取等号时有$L \sim \Lambda^{-3}$。
红外截断
考虑有效量子场论的能量不超过同样长度的黑洞的质量，极大能量密度由紫外截断除以相应的体积给出$\sim \Lambda^4$，那么总能量为$\sim L^3 \Lambda^4$。黑洞的质量为$M \sim LG^{-1} \sim L M_p^2$，所以要求$L^3 \Lambda^4 \lesssim LM_p^2$，取等号时有$L \sim \Lambda^{-2}$也有$\Lambda \sim M_p^{\frac{1}{2}}L^{-\frac{1}{2}}$，可以求得此时的最大熵为$S \sim L^3 \Lambda^3 \sim L^{\frac{2}{3}}M_p^{\frac{2}{3}} \sim S_{BH}^{\frac{3}{4}}$说明有效量子场论取不到极大熵，即量子场论只能描述黑洞的低能物理。

其核心为
$$
L^3 \Lambda^3 \leq (S_\text{BH})^\frac{3}{4}
$$

所以Li等人认为，宇宙中尺度为R的体积内的真空能不能超过同体积的黑洞质量
$$R^3 \rho_\Lambda\mathop{ \leqslant M_\rm{BH}}$$
其中$M_\rm{BH}=\frac{Rc^2}{G}$，取自然单位制$\hbar=c=1$，以及$M_p^2=1/ G$普朗克质量
$$
R^3\rho_\Lambda \leqslant RM_p^2
$$
则全息暗能量的能量密度为
$$
\rho_\Lambda=3c^2M_p^2 R^{-2}
$$
这里加入了一个系数$3c^2$，其中$c$是理论参数，在de Sitter宇宙中是1，好像和光速无关。在哈勃尺度$R \sim 1/H$时暗能量密度和实际数据一致。

---

基本的动机
- Casimir energy in de Sitter space
- Quantum uncertainty of transverse position
- Entanglement entropy from quantum information theory
- Dark energy from entropic force


--- 

2004 Li
全息暗能量的能量密度为
$$
\rho_\Lambda=3c^2M_p^2 L^{-2}
$$
取哈勃视界$L=1/H$
$$
\rho_\Lambda=3c^2M_p^2 H^{2}
$$
Friedmann方程，取$8\pi=1$和$M_p=\sqrt{1/G}$和$k=0$，得到
$$
3M_p^2H^2=\rho
$$
其中$\rho=\rho_m+\rho_\lambda$，所以
$$
\rho_m=3(1-c^2)M_p^2H^2
$$
所以
$$
\begin{align*}
\rho_m \sim H^2 \\
\rho_\Lambda \sim H^2
\end{align*}
$$
是一致的，因此对标度因子的演化
$$
\begin{align*}
\rho_m \sim a^{-3} \\
\rho_\Lambda \sim a^{-3}
\end{align*}
$$
也是一致的，因此得到$p_m=p_{\Lambda}=0$，和观测事实$p_\Lambda<-1/3$不符。鉴定为哈勃尺度不行，于是转而使用粒子视界
$$
R_H=a \int_0^t \frac{dt}{a}=a \int_0^a \frac{da}{Ha^2}
$$
暗能量密度为
$$
\rho_\Lambda=3 \alpha^2 M_p^2 a^{-2(1+\frac{1}{c})}
$$
由能量密度随尺度因子的变化
$$
\rho \sim a^{-3(1+w)}
$$
$$
w=-\frac{1}{3}+\frac{2}{3c}>-\frac{1}{3}
$$
所以也不行，转而选择未来事件视界
$$
R_h=a \int_t^{\infty}\frac{dt}{a}=a \int_a^\infty \frac{da}{Ha^2}
$$
暗能量密度为
$$
\rho_\Lambda=3 \alpha^2 M_p^2 a^{-2(1-\frac{1}{c})}
$$
$$
w=-\frac{1}{3}-\frac{2}{3c}>-\frac{1}{3}
$$
符合观测，但不合逻辑：为什么未来的因会导致今天的果


陈童老师认为有两点问题
问题有二：第一，暗能量问题其实也就是量子引力的真空能问题，而黑洞通常被认为是量子引力的激发态，和基态的真空能并没有关系，黑洞的质量通常也被认为是不包含基态真空能的，因此，用黑洞来限制量子引力基态的真空能实在是没有道理。
第二，感觉没有理由用红外尺度来限制局域场论的紫外能标，尤其是没有理由将这个能标限制到宇宙学常数这么低的水平上。相反，应该得到限制的是局域场论的适用尺度，也就是给定一个高的紫外能标，相应局域场论能适用的红外尺度要得到限制，不能太大。也就是说，问题在于局域场论的locality在量子引力的尺度上是不对的。

Tsallis entropy Dark energy
由
$$
L^3 \Lambda^3 \leq (S_\text{BH})^\frac{3}{4}
$$
Tsallis熵形式为
$$
S_\text{s}=\gamma A^\delta
$$
考虑让$S_\text{BH}=\gamma A^\delta$，红外截断为Hubble视界$L=H^{-1}$
$$
\Lambda^4 \leqslant \gamma(4\pi)^\delta L^{2\delta-4}
$$
有Friedmann方程和转移方程
$$
\begin{align*}
\begin{cases}
\rho_\text{D}=BH^{-2\delta+4} \\
\dot{\rho_\text{D}}+3H \rho_\text{D}(1+w_\text{D})=0
\end{cases}
\end{align*}
$$
暗能量组分及其导数
$$
\Omega_\text{D}=\frac{BH^{-2\delta+2}}{3m_p^2}
$$
$$
\Omega_\text{D}'=\frac{d \Omega_\text{D}}{d (\ln a)}=(-2\delta+2)\Omega_D\frac{\dot{H}}{H^2}
$$
声速
$$
v_s^2=\frac{(\delta-1)(\Omega_\text{D}-1)}{[1-(2-\delta)\Omega_\text{D}]^2}
$$
宇宙年龄略
结论：
$\delta=1$，回到Li讨论$w=0$Hubble视界情形
$\delta=2$，$\Lambda$情形
$\delta>1$不稳定$v_s^2<0$

Fractional Holographic Dark energy
Granda-Oliveros cutoff
$$
L=(\alpha H^2+ \beta H)^{-1/2}
$$
Nojiri-Odinstsov cutoff
$$
L=L(H, \dot{H}, \ddot{H},...,L_p,L_f,\dot{L}_p,\dot{L}_f)
$$
$L_p$和$L_f$分别是粒子视界和未来事件视界

fractional Wheeler-Dewitt eq
$$
S_h=CA^{\frac{2+\alpha}{2 \alpha}}
$$
只考虑哈勃视界作为截断
$$
L=H^{-1}
$$
$$
\Omega_D=c^2H^{\frac{\alpha-2}{\alpha}}
$$
$$
\Omega_D'=\frac{3(\alpha-2)(1-\Omega_D)\Omega_D}{2 \alpha=\Omega_D(3 \alpha-2)}
$$
和红移关系
$$
\left(\frac{\Omega_D}{\Omega_{D0}}\right)^\alpha \left(\frac{1-\Omega_D}{1-\Omega_{D0}}\right)^2-\alpha=(1+z)^{3(\alpha-2)}
$$

# 2. 黑洞熵、广义熵、纠缠熵
**$AdS_{d+1}​/CFT_d$​ 对偶性**: 在 $d+1$ 维反德西特空间中的引力理论与$d$维边界上的共形场论是对偶的。换句话说，在 $d+1$ 维 AdS 空间内的物理现象可以通过 $d$ 维 CFT 来描述，反之亦然。

这意味着，引力理论（通常是超弦理论或 M 理论）在一个高维时空内的行为可以等效地用一个低维的无引力场论来描述。特别是，五维 AdS 空间中的超引力理论可以与四维共形场论相联系，这是 AdS/CFT 对偶性最常见的应用之一。
- **反德西特空间 (AdS)**: 这是一个具有负常数曲率的时空，通常用于描述具有引力的时空。它是一种与我们熟悉的平坦空间（如闵可夫斯基空间）不同的时空结构，具有边界的曲率性质。
- **共形场论 (CFT)**: 这是一种量子场论，具有共形对称性。这意味着它在局部尺度变换下保持不变，即该理论在不同尺度上具有相同的性质。共形场论在统计力学和量子场论中有广泛的应用。

量子力学中纠缠熵
$$
S_A=-\rm{tr}_A \rho_A \log \rho_A
$$
其中
$$
\rho_A=\rm{tr}_B\ket{\Psi}\bra{\Psi}
$$
在一维多体量子系统中，临界情况的纠缠熵为
$$
S_A=\frac{c}{3}\log\left[\frac{L}{\pi a}\sin\left(\frac{\pi l}{L}\right)\right]
$$
非临界情况为
$$
S_A=\frac{c}{6}\mathcal{A}\log \frac{\xi}{a}
$$
其中$l$和$L$分别是$A$子系统和$A \cup B$的长度，$a$-中心荷，$\mathcal{A}$-边界点的数量，$\xi$-相关长度
对于有任意$d-1$维边界($\partial A \in \mathbb{R}^d$)的子系统$A$，在$\mathbb{R}\times S^d$上定义CFT中的纠缠熵$S_A$  (R-T公式)
$$
S_A=\frac{\rm{area\ of\ }\gamma_A}{4 G_N^{d+2}}
$$
其中$\gamma_A$是$\rm{AdS}_{d+2}$空间中的静态最小面，$4 G_N^{d+2}$是$d+2$维的牛顿常数。也就是说，对于只能看到子系统A的观者来说，$\gamma_A$是全息面。

AdS时空常用的坐标系有两种，分别为Global坐标和Poincare坐标，一下以d=1即3D AdS时空为例，在Global坐标中这样的时空坐标为$(t,\ \rho,\ \theta)$一个时间坐标一个径向坐标和一个角度旋转坐标

推导

$\rm{AdS}_{3}$时空中，最小面是连接边界的测地线
![[Pasted image 20240821123410.png]]
$\rm{AdS}_{d+2}$时空中，最小面为一个最小超曲面，可以是盘形的也可以是面形的
![[Pasted image 20240821123524.png]]

作为一个具体的限制，我们可以认为当最小表面包裹视界时，黑洞熵与 CFT 的纠缠熵相同。
若bulk区域内存在多个极值曲面，应选取其中最小面积的面作为RT面。

> [!NOTE] Bulk和Brane
> - **Brane** 是一个嵌入在bulk中的低维子空间。例如，弦理论中的 DDD 维 brane（也称为 D-brane）是这样的一个结构。brane通常局限于某些粒子或场（例如，电磁场）只能在brane上传播，而引力场等其他场可以在整个bulk中传播。
> - 在一些物理模型中，比如 **Randall-Sundrum 模型**，我们生活的宇宙被认为是一个四维的 brane，而 bulk 是包含这一 brane 的五维空间。

协变形式的纠缠熵HRT公式
$$
S(R)=\frac{\mathcal{A}(X_R)}{4 G \hbar}
$$
其中$\mathcal{A}$是bulk中与边界子区域R同源的极端HRT面$X_R$的面积

RT公式是最低阶的半经典贡献项，若考虑量子修正，需考虑bulk内有效场论的中量子涨落的贡献，也就是RT面与边界子区域围成的bulk区域内物质场的纠缠熵$S_\text{ent-bulk}$。2013年，Faulkner, Lewkowycz和 Maldacena三人提出含有一阶量子修正项的全息纠缠熵FLM公式
$$
S(R)=\frac{\mathcal{A}(X_R)}{4 g \hbar}+S_\text{ent-bulk}
$$
黑洞的广义熵
$$
S_\text{gen}=\frac{\text{Area}}{4G}+S_\text{out}
$$
其中$S_\text{out}$是视界外的物质场纠缠熵的贡献

> [!NOTE] 黑洞热力学四个定律
> - **零定律**: 黑洞的表面引力在事件视界上处处相等，类似于热力学中的温度平衡。
> - **第一定律**: 黑洞的质量变化可以表示为熵、角动量和电荷变化的函数，类似于能量守恒定律。
> - **第二定律**: 在任何经典物理过程中的黑洞熵（或者是事件视界的面积）不会减少，类似于热力学中的熵增原则。
> - **第三定律**: 不能通过有限的过程将黑洞的表面引力降至零，类似于无法达到绝对零度。

2014年，Engelhardt和Wall两人提出可以精确到任意阶量子修正的全息纠缠熵EW公式
$$
S(R)_\text{bdy}=\frac{\mathcal{A}(\chi_R)}{4G}+S_\text{ent-bulk}
$$
$\chi_R$是量子极端曲面，不同于$X_R$经典极端曲面（RT面）

黑洞精细熵
2019年，Penington，Almheiri-Engelhardt-Marolf和Maxfield等人将EW公式运用到时空中计算蒸发黑洞的精细熵，提出计算黑洞精细熵的半经典QES公式
$$
S_{gen}(X)=\frac{Area(X)}{4 G_N}+S_{semi}(\sum_X)
$$
满足page curve。违反了一般的黑洞热力学第二定律，但提出仍然满足广义的第二定律

Hawking辐射的精细熵island rule
$$
S_\text{Rad}=\min_x\left\{\text{ext}_x\left[\frac{Area(X)}{4G_N}+S_{semi}\left[\sum_{Rad}U \sum_{Island}\right]\right]\right\}  
$$


# 3. 模型的参数限制
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

限制无非是观测值和理论值的比较，从而限制模型里的参数。

SNIa型超新星爆发时质量在钱德拉塞卡极限附近，爆发时光度固定，可以计算得其绝对星等$M$
通过观测可以得到其视星等$m$
从而可以得到距离模数$\mu$
$$
\mu_{obs}=m-M
$$
另一方面，我们可以得到宇宙学理论的距离模数
$$
	\mu_{th}(z)=5\log_{10}d_L(z)+\mu_0,\ \mu_0=42.384-5\log_{10}h
$$
其中$h=H_0/100 Mpc \cdot km \cdot s^{-1}$，而光度距离为
$$
d_L(z)=(1+z)|\Omega_k|^{-1/2}sinn\{|\Omega_k|^{1/2}\int^z_0 \frac{cdz'}{H(z')}\}
$$

> [!NOTE] 光度曲线
> 光度曲线（light curve）是天文学中用于表示天体在一段时间内光度（亮度）变化的图表。横轴通常表示时间，纵轴表示光度（亮度）。

GRB
其爆发原因未完全知晓，采用和宇宙学无关的经验校正光度曲线从而估计出光度距离。

CBMF
一般认为，宇宙中超大质量星系团中包含的物质密度和宇宙平均物质密度相近，因此，其中重子物质与总物质之比也相当于宇宙重子能量密度和总能量密度之比。并且星系团中X射线气体主导，有比值
$$
f_{gas}=\frac{X射线气体质量}{总质量}=\frac{\Omega_b}{\Omega_m}
$$
和红移无关的量。人们通过原初核合成和CMB可以求出$\Omega_b$，运用观测得到的$f_{gas}$得到$\Omega_m$，p16

HUB
直接得出不同红移的哈勃参数值，因为$H(z)$是$w$的一次积分，运用星系的相对年龄来测量H
$$
	H \simeq -\frac{1}{1+z}\frac{\Delta z}{\Delta t}
$$
- $\Delta z$：两个星系之间的红移差，反映了它们在宇宙膨胀过程中受影响的程度差异。
- $\Delta t$：两个星系的年龄差，通常通过测量星系的光谱来确定。这一差异可以反映出宇宙膨胀历史的时间尺度。

CMB
CMB的温度涨落转化到球谐空间
$$
\frac{\delta T}{T}=\sum a_{lm}Y_{lm}
$$
对CMB的角功率谱进行限制
$$
C_l=\braket{|a_{lm}^2|}
$$

BAO
$z_d$是重子（普通物质）在宇宙历史上与光子的相互作用基本结束的时期
$$
r_d=\int_{z_d}^\infty \frac{c_s(z)}{H(z)}dz
$$
$$
D_M(z)=c \int_0^z \frac{dz'}{H(z')}
$$
$$
D_H(z)=\frac{c}{H(z)}
$$
通过限制

$$
\frac{D_M(z)}{r_d},\ \frac{D_H(z)}{r_d}
$$
BAO示意

![[Pasted image 20240828184414.png]]


