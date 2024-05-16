连续性方程：
$$
\partial_t \rho=-\nabla_r\cdot(\rho\vec{u})
$$
描述了在一个固定的体积中，只有一股粒子离开或进入这个体积（用质量的通量$\rho \vec{u}$反映）时，质量密度才会发生变化。

欧拉方程
$$
(\partial_t+\vec{u}\cdot \nabla_r)\vec{u}=\frac{\nabla_r P}{\rho}-\nabla_r \Phi
$$
这里面$D_t \boldsymbol{u}=(\partial_t+\boldsymbol{u}\cdot \nabla_r)\boldsymbol{u}$表示“对流时间导数”。$P=P(\rho,T)$是压强依赖于密度和温度的关系（又叫状态方程equation of state）。后面那一项是势的变化，表示外力。

接下来对$P$和$\rho$作微扰，其结果里带一横杠的是"背景数"（background values），有$\delta$的项是微扰部分
$$
\begin{align}
\rho(t,\boldsymbol{r}) & =\bar{\rho}(t)+\delta \rho(t,\boldsymbol{r}) \\
P(t,\boldsymbol{r}) & =\bar{P}(t)+\delta P(t,\boldsymbol{r})
\end{align}
$$
我们考虑一个静态的空间，忽略了引力$\Phi=0$然后把上面两个式子带进连续性方程和欧拉方程里，得到
$$
\begin{align}
\partial_t \delta \rho&=-\nabla_r \cdot(\bar{\rho} \boldsymbol{u}) \\
\bar{\rho}\partial_t \boldsymbol{u}&=\nabla_r \delta P
\end{align}
$$
上边两个式子结合一下（分别乘$\partial_t$和$\nabla_r$然后相加一下）可以得到
$$
\partial_t^2 \delta \rho - \nabla_r^2 \delta P=0 \tag{*}\label{eq1}
$$
这里我们想只用$\delta \rho$写这个式子的话，我们可以考虑正压的流体$P=P(\rho)$这样就可以把微扰重新写成
$$
\delta P =\frac{\partial P}{\partial\rho}\delta \rho \equiv c_s^2 \delta \rho
$$
这里面$c_s$就是流体的声速。
那我们$\eqref{eq1}$式子就可以变成
$$
(\partial_t^2-c_s^2 \nabla^2_r)\delta \rho=0
$$
这显然是一个波动方程，那么它的解自然就是
$$
\delta \rho(\boldsymbol{r},t)=\boldsymbol{A_k}\sin(wt-\boldsymbol{kx})+\boldsymbol{B_k}\cos(wt-\boldsymbol{kx})
$$
这里面有波矢（空间的频率）$\boldsymbol{k}$和频率（时间的频率）$w$


傅里叶空间