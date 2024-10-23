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


减速因子
 $$
q=\frac{d}{dt}\frac{1}{H}-1=-\frac{\ddot{a}a}{\dot{a}^2}=\frac{1}{2}(1+3w)=-\frac{\dot{H}}{H^2}-1$$

$$
\dot{H}=-H^2(1+q)
$$
 又因为
$$
\frac{d}{dt}=\frac{d}{dt}\frac{dt}{dz}=-(1+z)H(z)\frac{d}{dz}
$$ 所以减速因子又可以写成
$$
q(z)=-(1+z)H(z)\frac{d}{dz}\left(\frac{1}{H}\right)-1=(1+z)\frac{1}{H(z)}\frac{dH(z)}{dz}-1
$$
---

FLRW度规
$$
ds^2=-dt^2+a^2(t)\delta_{ij} dx^i dx^j
$$
理想流体的能动张量
$$
T_{\mu \nu}=pg_{\mu \nu}+(\rho+p)U_\mu U_\nu
$$

得到 Friedmann 方程（$p$和$\rho$在方程里是耦合的）
$$
\begin{align*}
\rho &=\frac{f}{2}-6f_Q H^2-\frac{2f_T}{1+f_T}(\dot{f}_QH+f_Q \dot{H}) \\
p &=-\frac{f}{2}+6f_Q H^2+2(\dot{f}_QH+f_Q \dot{H})
\end{align*}
$$
修改引力场作为有效密度和压强
$$
\begin{align*}
\rho_{\text{eff}}&=3H^2=\frac{f}{4f_Q}-\frac{1}{2f_Q}[(1+f_T)\rho+f_T p]\\
-p_{\text{eff}}&=2\dot{H}+3H^2=\frac{f}{4f_Q}-\frac{2\dot{f}_Q H}{f_Q}+\frac{1}{2f_Q}[(1+f_T)\rho +(2+f_T)p]
\end{align*}
$$
等效暗能量的EoS parameter（待验证）
$$
w_{\text{eff}}=\frac{p_{\text{eff}}}{\rho_{\text{eff}}} = \frac{f - 8\dot{f}_Q H + 2[(1 + f_T)\rho + (2 + f_T)p]}{f - 2[(1 + f_T)\rho + f_T p]}
$$
$$
w_{\text{eff}}=\frac{p_{\text{eff}}}{\rho_{\text{eff}}}=\frac{-f-[(1+f_T)\rho+(2+f_T)p]+8\dot{f}_QH}{f-[(1+f_T)\rho+f_Tp]}
$$
EoS parameter
$$
w=\frac{p}{\rho}=-1+\frac{4 f_Q H+f_Q \dot{H}}{(1+f_T)(f-12f_QH^2)-4 f_T(\dot{f}_QH+f_Q \dot{H})}
$$

deceleration parameter（自己计算的和其有出入）
$$
	q=-\frac{\ddot{a}a}{\dot{a}^2}=\frac{1}{2}(1+3w)=\frac{1}{2}\left(1+3\frac{p_{\text{eff}}}{\rho_{\text{eff}}}\right)=-1+\frac{3(4\dot{f}_QH-f+2p)}{f-2[(1+f_T)\rho+f_Tp]}
$$
我算出来的是
$$
q=-1+\frac{12\dot{f}_QH-6(1+f_T)(p+\rho)}{f-2[(1+f_T)\rho+f_Tp]}
$$
$p=p_{\text{de}}$，$\rho=\rho_m+\rho_{\text{de}}$

合并成H的演化
$$
\dot{H}+\frac{\dot{f}_Q}{f_Q}H=\frac{1}{2f_Q}(1+f_T)(\rho+p)
$$
假设
S. H. Shekh, Models of holographic dark energy in f ( Q ) gravity, Physics of the Dark Universe **33**, 100850 (2021).
$$
H=k(1+(1+z)^\alpha)
$$
$$
w=\frac{p}{\rho}=\gamma-1
$$
若$f=\alpha Q+\beta T$，$Q=6H^2$，$T=-\rho+3p$
进一步化简Friedmann（尚待验证）
$$
\begin{align*}
\rho &=-2\alpha H^2+ \alpha \dot{H}\left(\frac{1}{2}-\frac{5\beta}{3(1+\beta)}\right) \\
p&=2\alpha H^2+\alpha \dot{H}\left(\frac{1}{2}-\frac{\beta}{3(1+\beta)}\right)
\end{align*}
$$
从而有
$$
w=\frac{2H^2+\dot{H}(\beta+3)}{-2H^2+\dot{H}(-7\beta+3)}
$$
考虑哈勃截断的全息暗能量密度(这里用$\xi \rightarrow \alpha$防止符号重合)
$$
\rho_{de}=3H^2=k^2(1+(1+z)^\xi)^2
$$
则
$$
w=\frac{2\alpha H^2+\alpha \dot{H}\left(\frac{1}{2}-\frac{\beta}{3(1+\beta)}\right)}{k^2(1+(1+z)^\xi)^2}
$$





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


$$
w=\frac{2 \alpha(\dot{H}+3H^2)-3H^2}{k^2(1+(1+z)^\xi)^2}
$$
$$
w_\Lambda=-1+\frac{2(2-q)f_Q}{3}+\frac{2}{3}H \dot{f}_Q-m(6H)^{n-1}
$$
其中$f=Q+mQ^n$，$f_Q=\frac{d f}{d Q}=1+mnQ^{n-1}$，$\dot{f}_Q$是其对红移导数，$q=-1+\frac{\xi}{1+(1+z)^{-\xi}}$
$H=k(1+(1+z)^\xi)$，$Q=6H^2$

---
Friedmann方程
$$
\begin{align*}
\rho &=\frac{f}{2}-6f_Q H^2-\frac{2f_T}{1+f_T}(\dot{f}_QH+f_Q \dot{H}) \\
p &=-\frac{f}{2}+6f_Q H^2+2(\dot{f}_QH+f_Q \dot{H})
\end{align*}
$$
其中$f=\alpha Q+\beta T$，$Q=6H^2$，$T=-\rho+3p$，$w=\frac{p}{\rho}$，$H=k(1+(1+z)^\xi)$，$f_Q=\alpha$.

$$
w=\left(2-\frac{2\beta}{1+\beta}\right)\frac{\alpha \dot{H}}{3H^2\beta}-1
$$


