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
S_A=\frac{\rm{Area\ of\ }\gamma_A}{4 G_N^{d+2}}
$$
其中$\gamma_A$是$\rm{AdS}_{d+2}$空间中的静态最小面，$4 G_N^{d+2}$是$d+2$维的引力常数。也就是说，对于只能看到子系统A的观者来说，$\gamma_A$是全息面。

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
S_{gen}(X)=\frac{Area(X)}{4 G_N}+S_{semi}(\Sigma_X)
$$
满足page curve。违反了一般的黑洞热力学第二定律，但提出仍然满足广义的第二定律

Hawking辐射的精细熵island rule
$$
S_\text{Rad}=\min_x\left\{\text{ext}_x\left[\frac{Area(X)}{4G_N}+S_{semi}\left[\Sigma_{Rad}\cup\Sigma_{Island}\right]\right]\right\}  
$$

