- 单参微分同胚群：映射$\phi:\mathbb{R}\times M \rightarrow M$组成单参微分同胚群，满足
1. $\phi_t:M \rightarrow M$是微分同胚$\forall t \in \mathbb{R}$
2. $\psi_t \circ \phi_s=\psi_{t+s}, \forall t,s \in \mathbb{R}$
>其作为一个群，恒元是$\phi_0$，群乘法是复合映射，群元是$\phi_t$，群元的集合是$\{ \phi_t| t \in \mathbb{R} \}$

- 张量的对称部分和反称部分，以(0,2)阶张量为例子$$T_{(ab)}\coloneqq \frac{1}{2}(T_{ab}+T_{ba})$$ $$T_{[ab]}\coloneqq \frac{1}{2}(T_{ab}-T_{ba})$$
> 全反称和全对称表示张量只包含有反称部分或对称部分
- Killing矢量场：$(M, g_{ab})$上的矢量场$\xi^a$，若满足其给出的单参微分同胚群$\phi$是单参等度规群。
- 满足下面的Killing方程也是Killing矢量场的充要条件$$\nabla_a\xi_b+\nabla_b\xi_a=0$$
> Killing矢量场表现了空间的对称性

- 张量场：$\mathscr{F}_M(k,l)$表示在流形上的张量场
- 导数算符：映射$\nabla:\mathscr{F}_M(k,l)\rightarrow \mathscr{F}_M(k,l+1)$称为$M$上的导数算符（形式上是对偶矢量$\nabla_a$）

> Q： 导数算符的定义如此宽泛，想必一定有很多吧，那两个导数算符之间有什么关系？
> A：确实有很多，但导数算符作用在标量场是唯一的$$\nabla_a f=\tilde{\nabla}_a f=(df)_a$$
> 但作用在高阶的张量场上就不是这样的了，两者会相差一些东西
> 矢量$$\nabla_a v^b=\tilde{\nabla}_a v^b+C^b_{\ \ ac} v^c$$
> 二阶张量$$\nabla_a T^b_{\ \ c}=\tilde{\nabla}_a T^b_{\ \ c}+C^{b}_{\ \ ad}T^d_{\ \ c}-C^{d}_{\ \ ab}T^b_{\ \ d}$$
> 更一般的$$\nabla_a T^{b_1\dots b_k}_{\ \ \qquad c_1\dots c_l}=\tilde{\nabla}_a T^{b_1\dots b_k}_{\ \ \qquad c_1\dots  c_l}+\sum_j{C^{b_i}_{\ \ ad}T^{b_1\dots d\dots b_k}_{\ \ \qquad c_1\dots c_l}}\\-\sum_j{C^{d}_{\ \ ac_i}T^{b_1\dots b_k}_{\ \ \qquad c_1\dots d\dots c_l}},\quad \forall T\in\mathscr{F}_M(k,l)$$
>选取了具体的坐标系$\{x^\mu \}$后，我们选定“普通导数算符”$\tilde{\nabla}_a \equiv \partial_a$
>普通在什么地方呢？普通在作用在坐标轴的矢量基底和对偶矢量基底上都为0$$\partial_a(\partial/\partial x^v)^b=0,\quad\partial_a(d x^v)_b=0$$
>给定了普通导数算符后我们可以把$C^c_{\ \ ab}$写成$\Gamma^c_{\ \ ab}$就是我们常说的克氏符，此时相对于”普通“我们把$\nabla_a$叫做“协变导数算符”
>为`协变导数算符`和`普通导数算符`作用张量后的坐标分量分别引入新的记号：$$\begin{align}
T^\upsilon_{\ \ \sigma;\mu}=\nabla_\mu T^\upsilon_{\ \ \sigma} \\ T^\upsilon_{\ \ \sigma,\mu}=\partial_\mu T^\upsilon_{\ \ \sigma}
\end{align}$$
>分量关系式$$T^\upsilon_{\ \ \sigma;\mu}=T^\upsilon_{\ \ \sigma,\mu}+\Gamma^{\upsilon}_{\ \ \mu\alpha}T^\alpha_{\ \ \sigma}-\Gamma^{\alpha}_{\ \ \mu\sigma}T^\upsilon_{\ \ \alpha}$$
# 流形上的平移（包括矢量张量等）
什么是平移？所谓平移，就是矢量移动后不变。欧氏空间的平移是路径无关的，任意两个位置，平移的结果是唯一的。但在流形中，流形上的平移是路径依赖的。
所以为了推广，我们先研究在欧式空间中沿线$C(t)$平移
- 欧式空间的平移要求矢量平移后不变，即导数为0$$\frac{d v^a}{d t}=0$$
- 定义切矢$T^a=(\frac{\partial}{\partial x^\mu})^a T^\mu$，把切矢的定义放到上面的条件式中
$$\begin{aligned}0=\frac{d v^a}{d t} &=\frac{d x^\mu}{d t}\frac{\partial v^a}{\partial x^\mu} & \text{普通的矢量微分} \\ &=T^\mu \frac{\partial }{\partial x^\mu} v^a=T^\mu \partial_\mu v^a& \text{利用上面的切矢记号} \\ &=T^b \partial_b v^a & \text{重复抽象上下指标对应缩并} \end{aligned}$$
- 欧式空间中的方向导数：$T^b \partial_b v^a$即沿曲线的导数，在欧式空间中导数和方向导数都是0.

欧式空间的平移->流形上的平移
- 流形中的方向导数：$T^b \nabla_b v^a$
- 引入具体坐标$\{x^\mu \}$（抽象指标缩并->只剩下具体指标的分量）
$$\begin{align}
T^b\nabla_b v^a&=T_b(\partial_b v^a+\Gamma^a_{\ \ bc}v^c) \\
&=T^b[(dx^\nu)_b\left(\frac{\partial}{\partial x^\mu}\right)^a\partial_\nu v^\mu+\Gamma^a_{\ \ bc}v^c)]\\
&=\left(\frac{\partial}{\partial x^\nu}\right)^b T^\nu \left[(dx^\nu)_b\left(\frac{\partial}{\partial x^\mu}\right)^a\partial_\nu v^\mu+\Gamma^a_{\ \ bc}v^c)\right]\\
&=\left(\frac{\partial}{\partial x^\mu}\right)^a\left[T^\nu \partial_\nu v^\mu+\Gamma^\mu_{\ \ \nu\sigma} T^\nu v^\sigma \right] \\
&=\left(\frac{\partial}{\partial x^\mu}\right)^a\left(\frac{dx^\nu}{dt}\frac{\partial}{\partial x^\nu}v^\mu+\Gamma^\mu_{\ \ \nu\sigma} T^\nu v^\sigma\right)\\
&=\left(\frac{\partial}{\partial x^\mu}\right)^a\left(\frac{dv^\mu}{dt}+\Gamma^\mu_{\ \ \nu\sigma} T^\nu v^\sigma\right)
\end{align}
$$
- 联络：本来流形两个点的矢量空间互相无关，但有了协变导数算符之后可以通过某一条曲线联通两个矢量空间，所以把协变导数算符$\nabla_a$称为联络
- 与度规适配的导数算符：若$$\nabla_c g_{ab}=0$$则称算符为与度规适配的
> 在流形$M$上有了$\nabla_a$可以谈平移，再指定度规$g_{ab}$就可以谈内积了，在欧式空间中内积随平移不变，所以为了推广也要求流形上内积不变
> $$0=\frac{d}{dt}(g_{ab}u^a v^b)=T^c \nabla_c(g_{ab}u^a v^b)=u^a v^b T^c \nabla_c g_{ab}$$
> 由于这个条件对任意曲线和沿它平移的任意两个矢量，所以要求$$\nabla_c g_{ab}=0$$
- 度规适配的导数算符是唯一的
- 由于度规适配导数算符的唯一性，以后有度规时，我们谈导数算符都默认是指度规适配的。
- 度规流形中的克氏符$$\Gamma^c_{\ \ ab}=\frac{1}{2}g^{cd}[\partial_a g_{bd}+\partial_b g_{ad}-\partial_d g_{ab}]$$
- 度规流形中的克氏符分量$$\Gamma^\sigma_{\ \ \mu \upsilon}=\frac{1}{2}g^{\sigma \rho}[g_{\upsilon \rho,\mu}+g_{\mu \rho,\upsilon}-g_{\mu \upsilon,\rho}]$$
- 测地线：就是满足**切矢沿线平移**的特殊曲线$\gamma(t)$
- 测地线方程的坐标分量表达式$$\frac{d^2 x^\mu}{dt^2}+\Gamma^\mu_{\ \ \upsilon\sigma}\frac{d x^\upsilon}{dt} \frac{d x^\sigma}{dt} = 0$$
>根据其条件要求**切矢**沿线平移，而之前是一般矢量沿线平移，所以替换一下就行$$T^b\nabla_b T^a=0$$
>所以展开满足$$\frac{dT^\mu}{dt}+\Gamma^\mu_{\ \ \nu \sigma} T^\nu T^\sigma=0$$
>测地线的参数式是$x^\nu=x^\nu(t)$则$T^\nu=\frac{d x^\mu}{d t}$带入就得测地线方程。

- 坐标线
- 曲线的切矢
- 某点的坐标基矢就是是过该点坐标线的切矢
