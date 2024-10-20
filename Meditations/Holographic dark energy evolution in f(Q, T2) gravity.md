Evolution of  holographic dark energy models in $f(Q,T^2)$ gravity and cosmic constraint. 
$f(T)$ 
The existence of singularities presents a significant challenge in GR because they occur at high energy levels where GR is not valid due to quantum effects. [1]
To address this problem, 人们引入了energy–momentum squared gravity (EMSG)


 $f(Q)$是广义对称引力，Symmetric Teleparallel Gravity，曲率（curvature）和挠率（torsion）都是零，引力的几何性质通过“**非度量性**”（non-metricity）来描述。
 即，度量张量的协变导数不再为零。即非度规性
 $$
 Q_{\alpha \mu \nu}=\nabla_\alpha g_{\mu \nu}
$$
这也是weyl几何的性质，即不满足黎曼几何中的度规条件$\nabla_\alpha g_{\mu \nu}$，同时非度规性还可以写成
$$
Q_{\alpha \mu \nu}=-w_\alpha g_{\mu \nu}
$$
作用量变成
$$
S=\int d^4x \sqrt{-g} f(Q)
$$
是一种对称平行的引力（无曲无挠）
其中
$$
Q=-Q_{\alpha \mu \nu}P^{\alpha \mu \nu}
$$
其中
$$
\begin{align*}
P^\alpha_{\;\mu\nu} &\equiv \frac{1}{4}[-Q^{\;\ \  \alpha}_{(\mu\;  \nu)}+2Q^{\alpha}_{(\mu\nu)}+Q^\alpha g_{\mu \nu}-\tilde{Q}^\alpha g_{\mu \nu}-\delta^\alpha_{\;(\mu} Q_{\nu)}] \\
Q^\alpha & \equiv \\
\tilde{Q}^\alpha & \equiv \\
L^\alpha_{\;\beta \gamma}&\equiv \\

\end{align*}
$$
作用量
$$
S=\int(\frac{1}{16\pi}f(Q,T)+\mathcal{L}_m) \sqrt{-g}  d^4x 
$$
对作用量变分
$$
\begin{align*}
\delta S&=\int \left(\frac{1}{16 \pi} \delta[f(Q,T) \sqrt{-g}]+\delta(\mathcal{L}_m \sqrt{-g})\right)d^4x \\
&= \int \frac{1}{16\pi}\left(-\frac{1}{2}f g_{\mu\nu}\sqrt{-g}\delta g^{\mu\nu}+f_Q \sqrt{-g} \delta Q+f_T \sqrt{-g}\delta T -\frac{1}{2}T_{\mu \nu}\sqrt{-g}\delta g^{\mu\nu}\right)d^4x
\end{align*}
$$
其中
$$
T_{\mu\nu}\equiv -\frac{2}{\sqrt{-g}}\frac{\delta(\sqrt{-g}\mathcal{L}_m)}{\delta g^{\mu \nu}},\quad \Theta_{\mu \nu}\equiv g^{\alpha \beta}\frac{\delta T_{\alpha \beta}}{\delta g^{\mu \nu}}
$$
所以
$$
\delta T=\delta(T_{\mu \nu}g^{\mu \nu})=(T_{\mu \nu}+\Theta_{\mu \nu})\delta g^{\mu \nu}
$$

> [!NOTE] 一些推导
> $$
> \delta \sqrt{-g}=-\frac{1}{2}\frac{1}{\sqrt{-g}}\delta g=-\frac{1}{2}\frac{1}{\sqrt{-g}}g g^{\mu \nu}\delta g_{\mu \nu}=-\frac{1}{2}g_{\mu \nu}\sqrt{-g}\delta g^{\mu\nu}
> $$
> 第二个等号是行列式的变分，可参见https://zhuanlan.zhihu.com/p/74976891
> $$
> \delta g=g g^{\mu \nu}\delta g_{\mu \nu}
> $$
> 第三个等号是由于
> $$
> \delta(g^{\mu \nu}g_{\mu\nu})=\delta(4)=0=g^{\mu\nu}\delta g_{\mu \nu}+g_{\mu\nu}\delta g^{\mu \nu}
> $$
> 

场方程
$$
-\frac{2}{\sqrt{-g}}\nabla_\alpha(f_Q \sqrt{-g}P^\alpha_{\ \ \mu \nu})-\frac{1}{2}f g_{\mu \nu}+f_T(T_{\mu \nu}+\Theta_{\mu \nu})-f_Q(P_{\mu \alpha \beta}Q^\nu_{\ \ \alpha \beta}-2Q^{\alpha \beta}_{\ \ \ \ \mu}P_{\alpha \beta \nu})=8\pi T_{\mu \nu}
$$
在FLRW度规下有
$$
ds^2=-dt^2+a^2(t)\delta_{ij} dx^i dx^j
$$
减速因子
$$
q=\frac{d}{dt}\frac{1}{H}-1=-\frac{\ddot{a}a}{\dot{a}^2}
$$
又因为
$$
\frac{d}{dt}=\frac{d}{dt}\frac{dt}{dz}=-(1+z)H(z)\frac{d}{dz}
$$
所以减速因子又可以写成
$$
q(z)=-(1+z)H(z)\frac{d}{dz}\left(\frac{1}{H}\right)-1=(1+z)\frac{1}{H(z)}\frac{dH(z)}{dz}-1
$$

理想流体的能动张量


--- 
M. Sharif, M. Z. Gul, and I. Hashim, Cosmic evolution of Tsallis holographic dark energy model in f ( R , T 2 ) gravity, Physics of the Dark Universe **46**, 101606 (2024).


红外截断
hubble截断
$$
L=\frac{1}{H}
$$
Granda–Oliveros cut-off
$$
L=(\gamma_1 H^2+\gamma_2 \dot{H})^{-\frac{1}{2}}
$$
Reyni entropy

