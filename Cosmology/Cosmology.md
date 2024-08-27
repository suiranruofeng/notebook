物理坐标系$\boldsymbol{r}$表示真实的距离
共动坐标系$\boldsymbol{x}$表示剔除宇宙膨胀的距离
物理距离$\boldsymbol{r}$和共动距离$\boldsymbol{x}$之间的关系，标度因子$a(t)$
$$
\boldsymbol{r}=a(t)\boldsymbol{x}
$$
早期宇宙$a(t)$接近0，规定现在的标度因子$a_0(t_0)=1$

物理速度
$$
\boldsymbol{v}=\frac{d\boldsymbol{r}}{dt}=\frac{da\cdot \boldsymbol{x}}{dt}=\frac{\dot{a}}{a}\cdot a\boldsymbol{x} \equiv H(t)\boldsymbol{r}
$$
哈勃常数$H(t)=\frac{\dot{a}}{a}$
Hubble定律：物理速度与物理距离成正⽐
Q：理论上会超光速？
A：是这样，但不会违背SR，因为SR是说**相互路过**的两个物体的相对速度不能超过光速，不适⽤于远距离物体的相对速度。两个远距离物体之间没有光传播，**没有因果关系**。


宇宙膨胀的直接结果是遥远的地方天体发射的光会由于膨胀，在传播的过程中其波长被拉长，从而频率降低，产生红移现象，波长被拉长的距离应该是和宇宙的尺度成正比，宇宙尺度越大。
所以我们可以定义这样的现象，我们用一个延展的因子$z$来表示
$$1+z=\frac{\lambda_\rm{obs}}{\lambda_\rm{emit}}=\frac{a_\rm{obs}}{a_\rm{emit}}=\frac{1}{a_\rm{emit}}$$
这里取$a_\rm{obs}=1$表示我们现在看到的宇宙尺度，也是最大的，$a_\rm{emit}$都是比1小的。
我们也可以这样定义红移因子
$$z=\frac{\lambda_r-\lambda_e}{\lambda_e}=\frac{v}{c}$$
和尺度因子的关系$$\frac{\lambda_r}{\lambda_e}=\frac{a(t_r)}{a(t_e)}=1+z$$
当取$t_r=t_0$时，即现在时刻接收到光波$a(t_0)=1$
$$\frac{1}{a(t_e)}=1+z$$
首先我们想问宇宙是什么形状的，广义相对论告诉我们这由物质密度决定，只有封闭的、开放的、平坦的三种，如果处于临界密度，则正好是平坦的。想要这么准确的处于平坦是很难的，但所有观测都表面我们的宇宙是平坦的。
尺度因子$a$当然是可以随着时间变化的，我们为了了解宇宙的历史，自然想要知道它是怎么随时间变化的。广义相对论告诉了宇宙演化和能量的关系，所以尺度因子有如下的变化（推导在之后会讲）我们现在的宇宙$a=1$并且背景辐射的温度为2.7K，而宇宙最一开始是辐射主导的其随时间演化为$a\propto t^{1/2}$，之后在某一时间其随时间演化变为$a\propto t^{2/3}$。而恰好在最近的时间，宇宙变得由暗能量主导，随时间指数增长了。
![[Pasted image 20240813221527.png]]


- 共动坐标系
- 物理坐标系
- 宇宙时
- 共形时间$d\eta=dt/a(t)$


![[Pasted image 20240615104630.png]]



细调(Fine Tuning)问题是指物理理论中出现一些极度精细的参数或者量,这些参数必须被非常精确地调整到特定的狭窄范围内,才能使理论的预言与观测数据相符。这种精细的调节通常被认为是"不自然"的,可能暗示着我们所知的理论是不完整的。
宇宙学常数(cosmological constant)的细调问题 - 理论预言的值比观测值大约小10^120倍。



宇宙年龄（哈勃时间）
由$$
\dot{a}^2=H^2a^2=H_0^2 a^2(\Omega_m a^{-3}+\Omega_r^{-4}+\Omega_\Lambda+\Omega_k a^{-2})
$$
其中
$$
\Omega_{crit}=\frac{\rho_{i,0}}{\rho_{crit,0}},\ \rho_{crit}=\frac{3H_0^2}{8\pi G}
$$
于是可以从0积分到$t_0$求得宇宙的年龄
$$
t_0=\int_0^{t_0}dt=\int_0^1 \frac{da}{Ha}=\int_0^1 \frac{da}{H_0 a \sqrt{\Omega_m a^{-3}+\Omega_r^{-4}+\Omega_\Lambda+\Omega_k a^{-2}}}\approx138 \times 10^8 \mathrm{year}
$$
另外的写法
$$
t_0=\int_0^{t_0}dt=\int_0^1 \frac{da}{Ha}=\int \frac{1+z}{H}d \left(\frac{1}{1+z}\right)=\int_0^\infty H^{-1}\frac{1}{1+z}dz
$$
不考虑辐射、暗能量、曲率，只考虑物质时$\Omega_m=1$
$$
t_0=\frac{1}{H_0}\int_0^\infty \frac{1}{1+z}\frac{1}{\sqrt{(1+z)^3}}dz=\frac{2}{3H_0}
$$
运用上述的不考虑暗能量的宇宙年龄计算可观测宇宙半径的当今值，取了$a_0=1$，共形传播时间积分求得光的共形传播距离，再乘上现在的尺度因子得到
$$
d_0=a_0\int \frac{dt}{a}=\int \frac{da}{Ha^2}=\int \frac{(1+z)^2}{H}d\left(\frac{1}{1+z}\right)=\int_0^\infty H^{-1} dz=\frac{1}{H_0}\int_0^\infty \frac{1}{\sqrt{(1+z)^3}}dz=\frac{2}{H_0}
$$
因此有关系
$$
d_0=3t_0 \approx 42\mathrm{Gyr}
$$
哈勃视界
$$
d_H=\frac{1}{H_0}\approx 14 \mathrm{Gyr}
$$

可观测宇宙半径
$$
d=a(t)\int_{rec}^{t_0}\frac{dt}{a(t)}
$$
现在的可观测宇宙
$$
d_0=a_0 \int^{a_0}_{a_{rec}} \frac{da}{H_0a^2 \sqrt{\Omega_m a^{-3}+\Omega_r^{-4}+\Omega_\Lambda+\Omega_k a^{-2}}} \approx 46 \mathrm{Gyr}
$$
可以参考
[当今可观测宇宙半径怎么计算得到的? - 寻风的回答 - 知乎](https://www.zhihu.com/question/435774852/answer/1637909825)




宇宙学中的距离 待续
