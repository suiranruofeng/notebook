BH熵可以部分理解为跨越黑洞视界的纠缠熵

可观测值$O_a$的期望值为
$$
\braket{O_a}_p=\sum_a O_Ap_a
$$
shannon熵
$$
S(p_a)=\braket{-\ln p_a}_p=-\sum p_a \ln p_a
$$
当$S(p)=0$时，$p_a=\delta_{aa_0}$表面在$a_0$具有明确的值
香农熵不仅仅是检测不确定性，它还是我们无知程度的定量度量
特征1.广延的，具有可加性（对于两个独立的态）
$$
S(p_{AB})=S(P_A)+S(P_B)
$$
2.无噪声编码定理
系统的态可以用$\frac{S(p)}{\ln 2}$个二进制bit刻画

大写的字母下标表示观测量所有可能的状态/值，小写的下标表示某一具体的状态

边缘分布
$$
(p_A)_a=\sum_b (p_{AB})_{ab}
$$
条件概率
$$
(p_{A|b})_a=\frac{(p_{AB})_{ab}}{(p_B)_b}
$$
条件熵
$$
\braket{S(p_{A|b})}_{p_B}=S(p_{AB})-S(p_B)
$$

相互作用信息（mutual information）
$$
I(A:B)\coloneqq S(A)-H(A|B)=S(A)+S(B)-S(AB)
$$

![[Pasted image 20240901162428.png]]
$$
S(AB)\leqslant S(A)+S(B)
$$
是谓shannon的次可加性\

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
定义纠缠熵(冯诺依曼熵)只对于子系统$\mathcal{A}$
$$
S_{\mathcal{A}}=-Tr_\mathcal{A}(\rho_\mathcal{A}\log \rho_\mathcal{A})
$$
纠缠熵是量子信息论中的一个概念，衡量了一个系统的两个子系统之间的量子纠缠程度。
其本征值构成纠缠谱
$$
S_\mathcal{A}=-\sum_i \lambda_i \log \lambda_i
$$
$$
S_A=S_B
$$
说明纠缠熵不是广延量，不取决于每个区域的大小
更general的，纠缠熵由函数
$$
S=(T,L,l,\epsilon)
$$
Replica Trick
Euclidean approach，其基本思路是使用replica trick，把von Neumann熵的计算转变为n阶Renyi熵的计算，后者就相当于计算约化密度矩阵的n次方的trace。这个计算可以用虚时路径积分来处理，图像上看相当于是把n个时空的replica粘起来
$$
\Psi(\phi_0(x))=\int_{t_E=-\infty}^{\phi(t_E=0,x)=\phi_0(x)}D \phi e^{-S(\phi)}
$$
![[Pasted image 20240906001710.png]]
配分函数的等价性
$$
Z_{CFT}=Z_{AdS}
$$


![[Pasted image 20240903134202.png]]