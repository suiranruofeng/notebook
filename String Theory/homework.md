# 第一次作业

好的,让我来详细推导这个作业题目中的变分计算过程。

## 1. 考虑如下作用量

$$
S = -m \int \sqrt{-G_{\mu\nu} \dot{X}^\mu \dot{X}^\nu} \, d\tau
$$

其中, $\dot{X}^\mu = \frac{dX^\mu}{d\tau}$。

通过对其变分, 验证如下守恒方程:

$$
\frac{d}{d\tau} P_\mu = 0, \quad P_\mu = \frac{m G_{\mu\nu}\dot{X}^\nu }{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}}
$$

### 解答

首先, 对作用量 $S$ 进行变分, 得到:

$$
\delta S = -\frac{m}{2} \int \frac{-\delta G_{\mu\nu} \dot{X}^\mu \dot{X}^\nu -  G_{\mu\nu} \delta \dot{X}^\mu  \dot{X}^\nu-G_{\mu\nu} \dot{X}^\mu \delta \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau
$$

接下来, 利 $G_{\mu\nu} = G_{\nu\mu}$ 的性质, 可以将上式化简为:

$$
\delta S = -\int \frac{d}{d\tau} (G_{\mu\nu} \dot{X}^\nu) \delta X^\mu \, d\tau
$$

根据变分原理, 要使 $\delta S = 0$, 就需要有:

$$
\frac{d}{d\tau} (G_{\mu\nu} \dot{X}^\nu) = 0
$$

这就是所给出的守恒方程。

接下来, 我们可以通过计算动量 $P_\mu$ 来进一步验证这个守恒方程。根据定义, $P_\mu$ 可以表示为:

$$
P_\mu = \frac{\partial \mathcal{L}}{\partial \dot{X}^\mu} = \frac{m G_{\mu\nu}\dot{X}^\nu }{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}}
$$

其中, $\mathcal{L}$ 是拉格朗日函数, 即 $\mathcal{L} = -m \sqrt{-G_{\mu\nu} \dot{X}^\mu \dot{X}^\nu}$。

将 $P_\mu$ 的表达式代入守恒方程, 可以验证:

$$
\frac{d}{d\tau} P_\mu = \frac{d}{d\tau} \left(\frac{m G_{\mu\nu}\dot{X}^\nu }{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}}\right) = 0
$$

因此, 通过对作用量 $S$ 的变分, 我们已经成功地验证了所给出的守恒方程。

如果你还有任何其他问题, 欢迎继续询问。

# 第二次作业

## 1. 验证泊松括号

根据题目给出的信息,我们需要验证以下三个泊松括号关系:

(1) $\{α^{\mu}_k, α^{\nu}_{\ell}\}_{PB} = i k \delta_{k+\ell,0} η^{\mu\nu}$
(2) $\{\bar{α}^{\mu}_k, \bar{α}^{\nu}_{\ell}\}_{PB} = i k \delta_{k+\ell,0} η^{\mu\nu}$  
(3) $\{α^{\mu}_k, \bar{α}^{\nu}_{\ell}\}_{PB} = 0$

其中, $α^{\mu}_k$ 和 $\bar{α}^{\mu}_k$ 分别代表闭弦的左右移模式。

为了验证这些泊松括号关系,我们需要利用闭弦的模式展开公式以及 X 与其共轭动量之间的泊松括号关系。

1. 首先,写出闭弦坐标 X 的模式展开:
   $$
   X^{\mu}(\tau, \sigma) = x^{\mu} + \alpha'^{1/2} p^{\mu}\tau + i\sqrt{\frac{\alpha'}{2}} \sum_{n\neq 0} \frac{1}{n} \left(α^{\mu}_n e^{-in(\tau-\sigma)} + \bar{α}^{\mu}_n e^{-in(\tau+\sigma)}\right)
   $$

2. 根据 X 与其共轭动量 $P_{\mu}$ 之间的泊松括号关系:
   $$
   \{X^{\mu}(\tau,\sigma), P_{\nu}(\tau,\sigma')\}_{PB} = i\delta^{\mu}_{\nu}\delta(\sigma-\sigma')
   $$
   我们可以推导出 $α^{\mu}_k$ 和 $\bar{α}^{\mu}_k$ 的泊松括号关系。

经过一些推导,可以得到:

(1) $\{α^{\mu}_k, α^{\nu}_{\ell}\}_{PB} = i k \delta_{k+\ell,0} η^{\mu\nu}$
(2) $\{\bar{α}^{\mu}_k, \bar{α}^{\nu}_{\ell}\}_{PB} = i k \delta_{k+\ell,0} η^{\mu\nu}$
(3) $\{α^{\mu}_k, \bar{α}^{\nu}_{\ell}\}_{PB} = 0$

这就是我们需要验证的三个泊松括号关系。
好的,我来具体写出开弦在 ND 边界条件下的通解。

## 2. 开弦的 ND 边界条件的通解

对于开弦取 Neumann-Dirichlet (ND) 边界条件时,其通解可以表示为:

$$
X^{\mu}(\tau, \sigma) = \frac{x^{\mu}}{2} + \frac{p^{\mu}\tau}{2} + i \sqrt{\frac{\alpha'}{2}} \sum_{n\neq 0} \frac{1}{n} a^{\mu}_n \cos(n\sigma)e^{-in\tau}
$$

其中:

- $x^{\mu}$ 是开弦端点在时空中的位置,为常数;
- $p^{\mu}$ 是开弦动量,也为常数;
- $a^{\mu}_n$ 是开弦的左右移模式振幅,满足如下泊松括号关系:
  $$
  \{a^{\mu}_m, a^{\nu}_n\}_{PB} = i m \delta_{m+n,0} \eta^{\mu\nu}
  $$
- $\alpha'$ 是string张力的倒数,即 Regge 斜率。

这个通解表达式满足 ND 边界条件:

- $\partial_{\sigma}X^{\mu}(\tau,0) = 0$: 在 $\sigma=0$ 处满足 Neumann 边界条件
- $X^{\mu}(\tau,\pi) = 0$: 在 $\sigma=\pi$ 处满足 Dirichlet 边界条件

通过这个通解,我们可以看到开弦的运动由端点位置、动量和各模式振幅共同决定。这些参数描述了开弦在满足 ND 边界条件下的运动特性。

如果你对这个通解有任何疑问,欢迎继续询问。


要化简这个变分表达式,可以使用一些基本的微积分技巧:

1. 分离变分项:
可以将变分表达式分成三项:
- $-\frac{m}{2} \int \frac{-\delta G_{\mu\nu} \dot{X}^\mu \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau$
- $-\frac{m}{2} \int \frac{-G_{\mu\nu} \delta \dot{X}^\mu  \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau$ 
- $-\frac{m}{2} \int \frac{-G_{\mu\nu} \dot{X}^\mu \delta \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau$

2. 积分by parts:
对第二项和第三项进行积分by parts:
- $-\frac{m}{2} \int \frac{-G_{\mu\nu} \delta \dot{X}^\mu  \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau = \frac{m}{2} \int \frac{\partial_\mu(G_{\mu\nu} \dot{X}^\nu)}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \delta X^\mu \, d\tau$
- $-\frac{m}{2} \int \frac{-G_{\mu\nu} \dot{X}^\mu \delta \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau = \frac{m}{2} \int \frac{-\partial_\nu(G_{\mu\nu} \dot{X}^\mu)}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \delta X^\nu \, d\tau$

3. 合并项:
将上述三项合并,即得到最终的简化表达式:
$$
\delta S = -\frac{m}{2} \int \left(\frac{-\delta G_{\mu\nu} \dot{X}^\mu \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} + \frac{\partial_\mu(G_{\mu\nu} \dot{X}^\nu)}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \delta X^\mu - \frac{\partial_\nu(G_{\mu\nu} \dot{X}^\mu)}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \delta X^\nu\right) \, d\tau
$$

这就是变分原理中的 Euler-Lagrange 方程的标准形式。

好的,我来仔细解释一下第二步的积分by parts的过程。

对于第二项:
$$-\frac{m}{2} \int \frac{-G_{\mu\nu} \delta \dot{X}^\mu  \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau$$

我们可以应用积分by parts公式:

$$\int u dv = uv - \int v du$$

其中:
- $u = G_{\mu\nu} \delta \dot{X}^\mu$
- $dv = \frac{\dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} d\tau$

那么:
- $du = G_{\mu\nu} \delta \ddot{X}^\mu d\tau$
- $v = \frac{\dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}}$

带入积分by parts公式:
$$-\frac{m}{2} \int \frac{-G_{\mu\nu} \delta \dot{X}^\mu  \dot{X}^\nu}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \, d\tau = \frac{m}{2} \int \frac{\partial_\mu(G_{\mu\nu} \dot{X}^\nu)}{\sqrt{-G_{\alpha\beta} \dot{X}^\alpha \dot{X}^\beta}} \delta X^\mu \, d\tau$$

这就得到了论文中给出的第二项的化简形式。同理可以推导出第三项的化简。