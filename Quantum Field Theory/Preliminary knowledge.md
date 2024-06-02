# EL方程
Euler-Lagrange方程的推导
$$
\begin{align}
\delta S &= \int^{t_2}_{t_1} dt \delta L[q_i(t),\dot{q}_i(t)]=\int^{t_2}_{t_1} dt \left(\frac{\partial L}{\partial q_i}\delta q_i+\frac{\partial L}{\partial \dot{q}_i }\delta \dot{q}_i\right) \\
&=\int^{t_2}_{t_1} dt \left(\frac{\partial L}{\partial q_i}\delta q_i+\frac{\partial L}{\partial \dot{q}_i }\frac{d}{dt} q_i\right) \\
&=\int^{t_2}_{t_1} dt \left(\frac{\partial L}{\partial q_i}\delta q_i+\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{q}_i }\delta q_i\right)-\frac{d}{dt}\frac{\partial L}{\partial \dot{q}_i}\delta q_i\right) \\
&=\int^{t_2}_{t_1} dt \left(\frac{\partial L}{\partial q_i}-\frac{d}{dt}\frac{\partial L}{\partial \dot{q}_i}\right)\delta q_i+\left.\left(\frac{\partial L}{\partial \dot{q}_i }\delta q_i\right)\right|_{t_1}^{t_2}
\end{align}
$$
- 广义坐标
- 广义动量
- EL方程，是质点系统的经典运动方程
  $$\frac{d}{dt}\frac{\partial L}{\partial \dot{q}_i}-\frac{\partial L}{\partial q_i}=0$$
- 广义动量，把广义速度表示成$\dot{q}_i(q_i,p_i)$$$p_i \equiv \frac{\partial L}{\partial \dot{q}_i}$$
- 哈密顿量，通过Legendre变换定义的$$H(q_i,p_i)\equiv p_i\dot{q}_i-L$$
- $H$表示系统的总能量，即动能和势能的和
- Hamilton正则运动方程，是2n个一阶方程代替的n个二阶EL方程
  $$\dot{q}_i=\frac{\partial H}{\partial p_i},\quad \dot{p}_i=-\frac{\partial H}{\partial q_i}$$
- 正则变量：广义坐标和广义动量统称（在量子力学中体现为正则对易）
# 经典场论中的作用量原理
- 场论中的广义坐标是$\Phi (x,t)$，每一个空间点都是一个自由度，因此具有无限个连续自由度
- 场论中的拉格朗日量拉格朗日密度（场论中“密度”用的比较多）$$L=\int d^3x \mathcal{L}(x)$$
- 场论中的广义动量共轭动量密度（ 正则共轭场）
- 场论中的哈密顿量，哈密顿密度
- 场论中的正则运动方程
- 场论中的正则变量
# Noether定理、对称性与守恒定律
- Noether定理，如果系统有一种连续对称性，就必然存在一条对应的守恒定律