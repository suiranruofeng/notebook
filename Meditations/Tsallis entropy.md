三种热力学量
1. 广延变量：随着系统的尺寸（体积或面积）成比例地增长$\sim L^d$
2. 表征外部条件的变量：描述系统所处的外部条件，它们通常会随着系统特征线性维度变化$\sim L^\theta$
3. 能量变量：表示能量的量$\sim L^\epsilon$，其中$\epsilon = d+\theta$
广延变量（Extensive Variables）广延变量是那些与系统的大小（或物质的数量）成正比的物理量。如果将系统分割成两个相同的部分，每部分的广延变量值将是原系统的一半。例如，如果有两个相同的系统，它们的总质量是单个系统质量的两倍。
强度变量（Intensive Variables）强度变量是那些与系统的大小无关的物理量。如果将系统分割成两部分，每部分的强度变量值与原系统相同。例如，将一杯水分成两杯，水的温度和压力不会变化。

$L^{d-1},\ d>1$
$\ln d, \ d=1$

1 标准热力学系统
$$
\begin{align*}
&\theta=0 ，T、p、\mu、H强度量\\ 
&\epsilon=d ，G、U广延量
\end{align*}
$$
2 在长程相互作用下，经典多体哈密顿系统的热力学量表现出异常的缩放行为，
相互作用$\sim r^{-\alpha}$，$0\leq \alpha \leq d$，因此可以得到关系
$$
\begin{align*}
\theta=d-\alpha \\
\epsilon=2d-\alpha
\end{align*}
$$
这是因为这种相互作用导致系统的势能积分发散，从而使得玻尔兹曼–吉布斯分配函数无法收敛，也因此标准的BG理论无法适用。如牛顿引力体系。
3 在施瓦西3+1d黑洞中
$$
E \sim M_\mathrm{Bh}\sim L \Rightarrow \epsilon=1, \ \theta=1-d
$$
$$
\begin{align*}
当d=2,\ \theta=-1,\ T \propto L^{-1}\propto M_{BH}^{-1} \\
当d=3,\ \theta=-2,\ T \propto L^{-2}\propto M_{BH}^{-2}
\end{align*}
$$
存在一些直观的矛盾，应当把黑洞看成2d表面还是3d物体，前者符合Bekenstein–Hawking的规律？BG熵或者量子中的冯诺依曼熵都是$\propto L^2$的，满足area law
故而若一个系统可看成d-1维的，则可以用可加性熵$S_{BG}$描述，否则需要用一个非可加的熵泛函描述
4 在2d黑洞可以得到同样的结论

- 一些作者倾向于认为，对于复杂系统而言，熵并不一定满足热力学广延性（即熵与系统大小成比例增加）。他们可能认为在强关联或复杂系统中，标准的熵不必满足广延性。
- 但文中指出，这种观点是“有点奇怪的”（“kind of bizarre”），因为存在许多物理和数学事实表明，熵应具有广延性，尽管在某些复杂系统中，这种广延性可能以不同的形式表现出来。

强关联系统中的状态数大大减少，因此这些系统的热力学熵无法用通常的熵定义，而需要通过一种非可加性的熵来描述。这种熵不同于传统的熵概念，更适合描述具有强关联或强纠缠特性的复杂系统。

Tsallis entropy Dark energy
由
$$
L^3 \Lambda^3 \leq (S_\text{BH})^\frac{3}{4}
$$
Tsallis熵形式为
$$
S_\text{s}=\gamma A^\delta
$$
考虑让$S_\text{BH}=\gamma A^\delta$，红外截断为Hubble视界$L=H^{-1}$
$$
\Lambda^4 \leqslant \gamma(4\pi)^\delta L^{2\delta-4}
$$
有Friedmann方程和转移方程
$$
\begin{align*}
\begin{cases}
\rho_\text{D}=BH^{-2\delta+4} \\
\dot{\rho_\text{D}}+3H \rho_\text{D}(1+w_\text{D})=0
\end{cases}
\end{align*}
$$
Eos
$$
w_\text{D}=\frac{\delta-1}{(2-\delta)\Omega_\text{D}-1}
$$
减速因子
$$
q=-1-\frac{\dot{H}}{H^2}=\frac{1}{2}\left[\frac{(1-2\delta)\Omega_\text{D}+1}{1-(2-\delta)\Omega_\text{D}}\right]
$$
暗能量组分及其导数
$$
\Omega_\text{D}=\frac{BH^{-2\delta+2}}{3m_p^2}
$$
$$
\Omega_\text{D}'=\frac{d \Omega_\text{D}}{d (\ln a)}=(-2\delta+2)\Omega_D\frac{\dot{H}}{H^2}
$$
声速
$$
v_s^2=\frac{(\delta-1)(\Omega_\text{D}-1)}{[1-(2-\delta)\Omega_\text{D}]^2}
$$
宇宙年龄略
结论：
$\delta=1$，回到Li讨论$w=0$Hubble视界情形
$\delta=2$，$\Lambda$情形
$\delta>1$不稳定$v_s^2<0$

q代数
微分方程
$$
\frac{dy}{dx}=y
$$
其解为$y=e^x$
推广的微分方程
$$
\frac{dy}{dx}=y^q
$$
其解为
$$
y=[1+(1-q)x]^{\frac{1}{1-q}}\equiv \exp_q(x)
$$
$$
\braket{O_aO_b'}\left(\frac{1}{1+x}\right)
$$
$$
\begin{align*}

\end{align*}
$$