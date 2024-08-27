爱因斯坦场方程$$G_{\mu \nu}=R_{\mu \nu}-\frac{1}{2}R g_{\mu \nu}=\frac{8\pi G}{c^4}T_{\mu \nu}$$
场方程的各个分量
$$
\begin{align*}
&G^0_{\ 0}=-\frac{3}{c^2}\left[\left(\frac{\ddot{a}}{a}\right)^2+\frac{kc^2}{a^2R_0^2}  \right] \\
&G^i_{\ j}=-\frac{1}{c^2}\left[2\frac{\ddot{a}}{a}+\left(\frac{\dot{a}}{a}\right)^2+\frac{kc^2}{a^2R_0^2} \right]\delta^i_{\ j}
\end{align*}
$$
能动张量的各个分量
$$
\begin{align*}
&T^0_{\ \ 0}=-\rho \\
&T^i_{\ \ j}=p \delta^i_{\ j}
\end{align*}
$$
带入爱因斯坦方程可以分别得到Friedmann方程
$$
\begin{align*}
\left(\frac{\dot{a}}{a}\right)^2=\frac{8\pi G}{3}\rho-\frac{kc^2}{a^2R_0^2} \\
\frac{\ddot{a}}{a}=-\frac{4\pi G}{3}\left( \rho+\frac{3P}{c^2} \right)
\end{align*}
$$
其实也可以通过牛顿的方法求得，见Baumann书p47-48

协变守恒方程
$$
\nabla_\mu T^\mu_{\ \ \nu}=0
$$
可以推导(Baumann p38-39)出
$$
\dot{\rho}+3\frac{\dot{a}}{a}\left( \rho+\frac{p}{c^2}\right)=0
$$
Friedmann第一方程可以写成哈勃参数的形式$H$
$$
H^2=\frac{8\pi G}{3}\rho-\frac{kc^2}{a^2 R_0^2}
$$
定义临界能量密度，指现在时刻的能量密度$t_0$
$$\rho_{crit}=\frac{3H_0}{8\pi G}$$
各个物质组分的能量密度
$$\Omega_m=\frac{\rho_m}{\rho_{crit}},\Omega_r=\frac{\rho_r}{\rho_{crit}},\Omega_{de}=\frac{\rho_{de}}{\rho_{crit}},\Omega_k=\frac{k}{H_0^2}$$
宇宙的膨胀历史由哈勃参量$H(a)=\dot{a}(t)/a(t)$描述$$\frac{H^2}{H_0^2}=\frac{\Omega_m}{a^3}+\frac{\Omega_k}{a^2}+\frac{\Omega_r}{a^4}+\Omega_{de}$$
用状态参数参数化上面的式子
$$
\frac{d \ln a}{dt}\approx H_0 \sqrt{\Omega_i}a^{-\frac{2}{3}(1+w_i)}
$$
将$t$改成共形时间$\eta$
$$
\frac{d \ln a}{d \eta}\approx H_0 \sqrt{\Omega_i}a^{-\frac{1}{2}(1+3w_i)}
$$
积分可以得到
$$
a(\eta) \propto \eta^{2/(1+3w_i)}
$$
