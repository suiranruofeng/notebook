考虑一个晶格模型，纯态系统
$$
\ket{\Psi}\in \otimes_\alpha \mathcal{H}_\alpha
$$
对纯态体系，体系内所有粒子均遵循一套波函数。而对于混合态，体系中存在多种波函数
![[Pasted image 20240905132139.png]]
对于上图的系统有
$$
\otimes_\alpha \mathcal{H}_\alpha \cong \mathcal{H}_\mathcal{A} \otimes \mathcal{H}_\mathcal{A^c}
$$
约化密度矩阵
$$
\rho_\mathcal{A}=Tr_{\mathcal{A}^c}(\ket{\Psi}\bra{\Psi})
$$
定义纠缠熵
$$
S_{\mathcal{A}}=-Tr_\mathcal{A}(\rho_\mathcal{A}\log \rho_\mathcal{A})
$$
其本征值构成纠缠谱
$$
S_\mathcal{A}=-\sum_i \lambda_i \log \lambda_i
$$

在d维时空中,自由无质量标量场的两点关联函数为$$$\langle\phi(x)\phi(y)\rangle = \frac{\Omega_d}{|x-y|^{d-2}}$$
其中
$$\Omega_d = \Gamma((d-2)/2)/(4\pi^{d/2})$$是d维时空的几何因子
在d维时空中,纠缠熵的典型行为为
$$S \sim A(\Sigma)\epsilon^{d-2}$$
这里$A(\Sigma)$是分割面$\Sigma$的面积,$\epsilon$是紫外截断
