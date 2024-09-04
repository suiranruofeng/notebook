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



![[Pasted image 20240903134202.png]]