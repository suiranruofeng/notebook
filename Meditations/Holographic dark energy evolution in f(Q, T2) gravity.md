Evolution of  holographic dark energy models in $f(Q,T^2)$ gravity and cosmic constraint. 
$f(T^2)$ 
The existence of singularities presents a significant challenge in GR because they occur at high energy levels where GR is not valid due to quantum effects. [1]
To address this problem, 人们引入了energy–momentum squared gravity (EMSG)

广义的仿射联络（general affine connection）
$$
\Gamma^\alpha_{\ \mu \nu}=\hat{\Gamma}^\alpha_{\ \mu \nu}+K^\alpha_{\ \mu \nu}+L^\alpha_{\ \mu \nu}
$$
其中$\hat{\Gamma}^\alpha_{\ \mu \nu}$是Levi-civita联络，具有无挠性和度规相容性$\nabla g=0$,
$$
\hat{\Gamma}^\alpha_{\ \mu \nu}=\frac{1}{2}g^{\alpha \beta}(\partial_\mu g_{\beta \nu}+\partial_\nu g_{\beta \mu}-\partial_\beta g_{\mu \nu})
$$
$K^\alpha_{\ \mu \nu}$是contortion tensor，满足
$$
 K^{\alpha}_{\,\,\mu\nu} =\frac{1}{2}T^{\alpha}_{\,\,\mu\nu} +T^{\,\,\,\alpha}_{(\mu\,\,\,\nu)} 
$$
其中$T^{\alpha}_{\,\,\mu\nu}$是挠率张量
$L^{\alpha}_{\,\,\mu\nu}$是disformation tensor，满足
$$ L^{\alpha}_{\,\,\mu\nu} = \frac{1}{2}Q^{\alpha}_{\,\,\mu\nu}-Q^{\,\,\,\alpha}_{(\mu\,\,\,\nu)}$$
其中$Q^{\alpha}_{\,\,\mu\nu}$是nonmetricity tensor
$$
\begin{align*}
Q_{\rho \mu \nu} &\equiv \nabla_{\rho} g_{\mu\nu} = \partial_\rho g_{\mu\nu} - \Gamma^\beta{}_{\rho\mu} g_{\beta\nu} - \Gamma^\beta{}_{\rho\nu} g_{\mu\beta}~, \\
T^{\lambda}{}_{\mu\nu} &\equiv
 \Gamma^{\lambda}{}_{\mu\nu}\!-\!\Gamma^{\lambda}{}_{\nu\mu}~ ,\\
 R^{\sigma}{}_{\rho\mu\nu} &\equiv \partial_{\mu} \Gamma^{\sigma}{}_{\nu\rho}\! - \! \partial_{\nu} \Gamma^{\sigma}{}_{\mu\rho}\! +\! \Gamma^{\alpha}{}_{\nu\rho}  \Gamma^{\sigma}{}_{\mu\alpha} \!-\!\Gamma^{\alpha}{}_{\mu\rho} \Gamma^{\sigma}{}_{\nu\alpha}~ , 
\end{align*}
$$

 $f(Q)$是广义对称引力，Symmetric Teleparallel Gravity，曲率（curvature）和挠率（torsion）都是零，引力的几何性质通过“**非度量性**”（non-metricity）来描述。
 即，度规张量的协变导数不再为零。即非度规性
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
S=\int(\frac{1}{2}f(Q,T)+\mathcal{L}_m) \sqrt{-g}  d^4x 
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
上面两式combined，得出H的演化
$$
\dot{H}+\frac{\dot{f}_Q}{f_Q}H=\frac{1}{2f_Q}(1+f_T)(\rho+p)
$$
这个方程里面包含了H的信息，为了得到H的具体形式，我们需要知道$p$和$\rho$的具体式子，然后解微分方程，对于物质和暗能量有$p=p_{\text{de}}$，$\rho=\rho_m+\rho_{\text{de}}$
而$\rho_m$可以从Friedmann方程中得到，当然这需要我们知道$f$的具体式子，我们讨论第一种情况$f=\alpha Q+\beta T$，以及用$w_{\text{de}}p_{\text{de}}=\rho_{\text{de}}$得到$\rho_m,\rho_{\text{de}}$和$H，w_{\text{de}}$的关系式。但是未知数还是有两个$H，w_{\text{de}}$，我们其实只用了一个方程的信息并且假定$\rho_{de}$是全息暗能量
一共四个未知变量，$\rho_m,\rho_{de},H,p_{de}$，而我们有两个方程，一个假设，消去三个自由度
修改引力场作为有效密度和压强
$$
\begin{align*}
\rho_{\text{eff}}&=3H^2=\frac{f}{4f_Q}-\frac{1}{2f_Q}[(1+f_T)\rho+f_T p]\\
-p_{\text{eff}}&=2\dot{H}+3H^2=-\frac{f}{4f_Q}+\frac{2\dot{f}_Q H}{f_Q}-\frac{1}{2f_Q}[(1+f_T)\rho +(2+f_T)p]
\end{align*}
$$
等效暗能量的EoS parameter（mma计算得出）
$$
w_{\text{eff}}=\frac{p_{\text{eff}}}{\rho_{\text{eff}}} = \frac{f - 8\dot{f}_Q H + 2[(1 + f_T)\rho + (2 + f_T)p]}{f - 2[(1 + f_T)\rho + f_T p]}
$$
EoS parameter（好像没什么意义，表示宇宙所有组分的状态）
$$
w=\frac{p}{\rho}=-1+\frac{4 f_Q H+f_Q \dot{H}}{(1+f_T)(f-12f_QH^2)-4 f_T(\dot{f}_QH+f_Q \dot{H})}
$$

deceleration parameter（自己计算的和其有出入，不知道文献怎么得出的，两篇文献皆不相同）
$$
	q=-\frac{\ddot{a}a}{\dot{a}^2}=\frac{1}{2}(1+3w)=\frac{1}{2}\left(1+3\frac{p_{\text{eff}}}{\rho_{\text{eff}}}\right)=-1+\frac{3(4\dot{f}_QH-f+2p)}{f-2[(1+f_T)\rho+f_Tp]}
$$
我算出来的是
$$
q=-1+\frac{12\dot{f}_QH-6(1+f_T)(p+\rho)}{f-2[(1+f_T)\rho+f_Tp]}
$$
现在讨论一下几个解，就是$H$的具体形式，从而为了可以进行参数限制，我们可以直接把$w_{de}$看作参数，这样就消去一个自由度，结合全息暗能量的假设，就可以解出$H$
总的物质密度，假设$\rho=p (\gamma-1)$
$$
\rho=\rho_m+\rho_{de}=\frac{f-12f_Q H^2}{2(1+\gamma f_T)}
$$
---
$$
\boxed{\begin{align*}
3H^2&=\frac{f}{4f_Q}-\frac{1}{2f_Q}[(1+f_T)\rho+f_T p]\\
2\dot{H}+3H^2&=-\frac{f}{4f_Q}+\frac{2\dot{f}_Q H}{f_Q}-\frac{1}{2f_Q}[(1+f_T)\rho +(2+f_T)p]
\end{align*}
}
$$
0) 标准宇宙学 $\rho_{de}=3c^2 H^2$   
$$
H(z)=H_0(\Omega_m(1+z)^3+(1-\Omega_m)(1+z)^{3(1+w_{de})})
$$
$$
w_{de}=-\frac{2\dot{H}+3H^2}{3c^2H^2}
$$
$$
H(z)=H_0(\Omega_m(1+z)^3+(1-\Omega_m)(1+z)^{-\frac{2\dot{H}}{H^2}})
$$
$$
2\dot{H}+w_{de}3c^2H^2=0
$$
$$
H(z)=\frac{1}{3c^2w_{de}t-c_0}
$$
$$
\begin{align*}
&H_0=\frac{1}{3c^2w_{de}t_0-c_0}\\
&c_0=-\frac{1}{H_0}+3c^2w_{de}t_0 \\
&H(z)=\frac{H_0}{H_03c^2w_{de}(t-t_0)+1}\\
&\frac{\dot{a}}{a}=\frac{H_0}{H_03c^2w_{de}(t-t_0)+1}\\
&a(t)=c_2(1+3c^2H_0(t-t_0)w_{de})^{\frac{1}{3c^2w_{de}}}\\
&a(t)=a_0(1+3c^2H_0(t-t_0)w_{de})^{\frac{1}{3c^2w_{de}}}
\end{align*}
$$

1) $f=\alpha Q$，以及哈勃视界作为截断的全息暗能量，此时$f_Q=\alpha,f_T=0,f=6\alpha H^2,\rho_{de}=3c^2H^2$
$$
\begin {align}
\begin {cases}
3H^2=\frac{6 \alpha H^2}{4 \alpha}-\frac{1}{2\alpha}\rho \\
2\dot{H}+3H^2=-\frac{6\alpha H^2}{4\alpha}-\frac{1}{2\alpha}(\rho+2p)
\end{cases}
\end{align}
$$
=>
$$
\begin{align*}
p_{de}&=-(2\alpha \dot{H}+3 \alpha H^2) \\
\rho_{de}&=3c^2H^2 \\
w_{de}&=-\frac{2 \alpha \dot{H}+3\alpha H^2}{3c^2H^2}
\end{align*}
$$
哈勃参数的演化$\rho \propto (1+z)^{3(1+w)}$
$$H(z)=H_0(\Omega_m(1+z)^3+(1-\Omega_{m})(1+z)^{\frac{(3-3 \alpha) H^2-2\alpha \dot{H}}{H^2}})$$
两个没什么用的计算where $\gamma=w+1$
$$
\rho=\frac{f-12FH^2}{2}
$$
$$
\dot{H}=\frac{\gamma}{2\alpha}\rho=\frac{\gamma(f-12FH^2)}{4\alpha}=-\frac{3}{2}\gamma H^2
$$
2) $f=\alpha Q+ \beta T=6\alpha H^2+\beta(-\rho+3p), \rho_{de}=3H^2$且$\alpha,\beta$都是和时间无关的参数，$f_Q=\alpha,f_T=\beta$
由演化方程得到
$$
\dot{H}=\frac{1}{2\alpha}(1+\beta)(\rho_m+\rho_{de}+p_{de})
$$
由Friedmann第二个式子得到
$$
(2+3\beta)p_{de}=6 \alpha H^2+4 \alpha \dot{H}+\beta \rho_m+\beta \rho_{de}
$$
带入关系式$p_{de}=\rho_{de}w_{de}$，得到物质的能量密度
$$
\rho_{m}=\frac{2 \alpha \dot{H}}{1+\beta}-\rho_{de}(1+w_{de})
$$
将上述三个式子合并得
$$
\begin{align*}
(2+4\beta)\rho_{de}w_{de}=\left(6\alpha H^2 + 4\alpha \dot{H}+\frac{2 \alpha \beta \dot{H}}{1+\beta}\right)\\
(2+4\beta)3H^2w_{de}=\left(6\alpha H^2 + 4\alpha \dot{H}+\frac{2 \alpha \beta \dot{H}}{1+\beta}\right)\\
[6(1+2\beta)w_{de}-6 \alpha]H^2-4 \alpha \dot{H}=\frac{2 \alpha \beta \dot{H}}{1+\beta}
\end{align*}
$$
$$
w_{de}=\frac{\frac{4 \alpha+6 \alpha \beta}{1+\beta}\frac{\dot{H}}{H}+6\alpha}{6(1+2\beta)}
$$
3) $f=m Q^n+\beta T$


S. H. Shekh, Models of holographic dark energy in f ( Q ) gravity, Physics of the Dark Universe **33**, 100850 (2021).
假设
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


$$
\dot{H}+\frac{3(\alpha+1)}{(3\alpha+2)}[H^2+(2\alpha+1)c^2 w_h H^2]=0
$$
$$
H = \left((2a + 1)c^2 \omega_h H_0 e^{-\frac{3(1+\alpha)(2a+1)c^2 \omega_h (t-t_0)}{(3a+2)}}\right)
$$
$$
H(z) = \frac{H_0 - (2a + 1)\omega_h c^2\left[(1 + z)^{-\frac{3(a+1)}{(3a+2)}} - 1\right]}{(1 + z)^{-\frac{3(a+1)}{(3a+2)}}}
$$
$$\begin{align}  
f + Q - 2Qf_Q = 2\rho \\  
H = \frac{\rho + p}{2(-1 + f_Q + 2Qf_{QQ})}  
\end{align}$$
These Eqs. (20) and (21) can be interpreted as symmetric teleparallel equivalent to GR (STG) cosmology with an additional component arising due to non-metricity of space-time which behaves like dark energy fluid part. These dark energy fluid components evolving due to non-metricity are defined by

$$\begin{equation}  
\rho_{\text{DE}} = -\frac{f}{2} + Qf_Q  
\end{equation}$$

and

$$\begin{equation}  
p_{\text{DE}} = -\rho_{\text{DE}} - 2H(f_Q + 2Qf_{QQ})  
\end{equation}$$
---
f(R,T)
$$
H = ((2\alpha + 1)c^2\omega_H H_0)e^{-\frac{3(1+\alpha)(2\alpha+1)c^2\omega_H (t-t_0)}{(3\alpha+2)}}/
\left(((2\alpha + 1)c^2\omega_H) + H_0\left(1 - e^{-\frac{3(1+\alpha)(2\alpha+1)c^2\omega_H (t-t_0)}{(3\alpha+2)}}\right)\right)
$$

$$
\frac{\alpha  2^{n-1} 3^{n-2} \left(H(t)^2\right)^{n-2} \left(2 n (-2 \beta +(3 \beta +2) n-1) H'(t)+3 (\beta +1) (2 n-1) H(t)^2\right)}{(\beta +1) (2 \beta +1) c^2}
$$
$$\frac{2 \alpha  3^{n-2} \left(\text{H0}^2 \left((z+1)^{2 m}+1\right)\right)^{n-2} \left(\frac{3}{2} (\beta +1) \text{H0}^2 (2 n-1) \left((z+1)^{2 m}+1\right)+\frac{\sqrt{2} \text{H0} m n (z+1)^{2 m-1} (-2 \beta +(3 \beta +2) n-1)}{\sqrt{(z+1)^{2 m}+1}}\right)}{(\beta +1) (2 \beta +1) c^2}$$




$$\omega_\Lambda = \frac{p_\Lambda}{\rho_\Lambda} = \frac{\alpha}{3}\left(-6\right)^n\left[\frac{H_0}{\sqrt{2}}\left(\sqrt{1 + (1 + z)^{2m}}\right)\right]^{2n-2}\left(n - \frac{1}{2}\right) - \frac{\alpha n }{9} \frac{H_0^2}{2}m(1 + z)^{2m}\left(-6\right)^n H^{2n-4}(2n - 1).$$

prev
$$
p_{de}=\left[\frac{2\beta}{1+\beta}(n+1)+\frac{2}{3}\alpha n(2n-1)6^n\right]\dot{H}+(2\alpha n-\alpha)(6H^2)^n
$$
$$
    w_{de}=\frac{p_{de}}{\rho_{de}}=\frac{-\frac{1}{2}\left[\frac{2\beta}{1+\beta}(n-1)+\frac{2}{3}\alpha n(2n-1)6^n\right]\dot{H}-\frac{1}{2}\alpha(2n-1)(6H^2)^n}{3c^2H^2}
$$

$$
q=-1+\frac{1+\alpha}{e^{\beta t}}
$$
---
$$
\frac{\alpha(2n(-2\beta+(3\beta+2)n-1))6^{n-1}((2n-2)H^{2n-3}\dot{H}^2+\ddot{H}H^{2n-2})+\alpha3(\beta+1)(2n-1)6^{n-1}2nH^{2n-1}\dot{H}}{6c^2H \dot{H}(\beta+1)(2\beta+1)}
$$

$$
H(z)=\frac{H_0}{\sqrt{2}}\sqrt{1+(1+z)^m}
$$