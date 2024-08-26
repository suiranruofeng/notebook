Holographic Derivation of Entanglement Entropy from the anti–de Sitter Space/Conformal Field Theory Correspondence
Shinsei Ryu and Tadashi Takayanagi

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

$\rm{AdS}_{3}$时空中，最小面是连接边界的测地线
![[Pasted image 20240821123410.png]]
$\rm{AdS}_{d+2}$时空中，最小面为一个最小超曲面，可以是盘形的也可以是面形的
![[Pasted image 20240821123524.png]]

作为一个具体的限制，我们可以认为当最小表面包裹视界时，黑洞熵与 CFT 的纠缠熵相同。


