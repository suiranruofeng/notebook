无论是SN Ia还是BAO、CMB其参数限制的参数简并方向都是不同的，它们单独对参数的限制并不强，因此需要进行联合的参数限制。我们可以定义总的观测函数
$$\chi^2_\rm{tot}=\chi^2_\rm{SN}+\chi^2_\rm{BAO}+\chi^2_\rm{CMB}$$
于是可以获得联合后验概率密度分布
$$\mathcal{P}(\theta|D)=\mathcal{L}(D_\rm{SN}|\theta)\times\mathcal{L}(D_\rm{BAO}|\theta)\times\mathcal{L}(D_\rm{CMB}|\theta)\times\pi(\theta)$$
其中$D$表示数据。$\theta$表示模型的参数，也是我们所要限制的。

MCMC采样原理
在参数空间中选取一个点作为起始点，并通过多次迭代到达最佳拟合点的位置，在这段时间内的采样不能真实的表示目标分布函数；还需要进行进一步的迭代来使所生成的参数进入平衡状态，并且把一开始的采样删掉从而提高采样的质量称为burn-in过程。

工具cosmoMC和在其基础上开发的cobaya



Fisher矩阵

