广义相对论可以用三种等效的数学几何形式描述
1 曲率$\Rightarrow f(\mathcal{R})$
2 挠率 torsion$\Rightarrow f(T)$
3 非度量 non-metric$\Rightarrow f(Q)$
通过修改Eninstain-Hilbert作用量
$$
S=\frac{1}{2k}\int R \sqrt{-g}d^4x
$$


比如$f(Q,T)$
修改成
$$
S=\int\left[\frac{1}{16\pi}f(Q,T)+\mathcal{L}_m\right]\sqrt{-g}d^4x
$$
通过变分求得修改后的场方程
![[Pasted image 20240906005137.png]]
并和FRW度规共同得出Friedmann eq?
![[Pasted image 20240906004959.png]]
$\kappa$是参数一般为1 $\tilde{G}=f_T,F=f_Q$ 取$f(Q,T)=\alpha Q+ \beta T$
另一方面
$$
H(z)=H_0[\Omega_{0m}(1+z)^3+(1-\Omega_{0m})]^{1/2}
$$
Barrow entropy
$$
S_b=\left(\frac{A}{A_0}\right)^{1+\frac{\Delta}{2}}
$$
$$
\rho_D=\frac{S_b}{L^4}\sim L^{2+\Delta-4}=CL^{\Delta-2}
$$
运用全息暗能量理论和哈勃视界IR截断
$$
L=\frac{1}{H(z)}
$$
$$
\rho_D=C\left(H_0\sqrt{\Omega_{0m}(z(z+3)+3)z+1}\right)^{2-\Delta}
$$
结合场方程也可以求得p
$$
p_D=-\frac{3 \alpha H_0^2\left(2(\Omega_{0m}-1)+\beta(\Omega_{0m}(z^3+3z^2+3z+3)-2)\right)}{4\beta^2+6\beta+2}
$$
以及相应的$w$

---

$f(\mathcal{G},T)$
$$
S=\int d^4x \sqrt{-g}\left(\frac{R+f(\mathcal{G},T)}{2k^2}+\mathcal{L}_m\right)
$$
$$
T=g_{\xi \eta}T^{\xi \eta}
$$

Gauss-Bonnet (GB) 不变量是二次曲率不变量的特殊线性组合
$$\mathcal{G} =\left(R^2 - 4R_{\mu\nu}4R^{\mu\nu} + R_{\mu\nu\rho\sigma}R^{\mu\nu\rho\sigma}\right)$$
变分
![[Pasted image 20240906011315.png]]
其中$\Theta_{\xi \eta}=g^{\mu \nu}(\delta T_{\mu \nu}/\delta g^{\xi \eta})$
$$
T_{\xi \eta}=-\frac{2}{\sqrt{-g}}\frac{\delta(\sqrt{-g}\mathcal{L}_m)}{\delta g^{\xi \eta}}
$$
考虑理想流体
$$
T_{\xi \eta}=(p+\rho)V_{\xi}V_{\eta}-pg_{\xi \eta},\ \  \Theta=-2T_{\xi \eta}-pg_{\xi \eta}
$$
能动张量的迹
$$
T=\rho-3p,\ \ \mathcal{G}=24H^2(\dot{H}+H^2)
$$
考虑场方程和FRW度规
![[Pasted image 20240906014422.png]]
取
$$
f(\mathcal{G},T)=F(\mathcal{G})+\chi T
$$
考虑幂率变化的尺度因子
$$
a(t)=a_0(\tau-t)^\lambda
$$
最后可以得到
![[Pasted image 20240906020923.png]]

同时选择barrow entropy 和未来事件视界
$$
S_b=\left(\frac{A}{A_0}\right)^{1+\frac{\Delta}{2}}
$$
$$
\rho_D=\frac{S_b}{L^4}\sim L^{2+\Delta-4}=CL^{\Delta-2}
$$
$$
R_h=a \int_t^{\infty}\frac{dt}{a}=a \int_a^\infty \frac{da}{Ha^2}
$$
得到EoS
$$
w_\Lambda=-\frac{1}{3}\left(\frac{2\sqrt{\Omega_\Lambda}}{c}+1\right)
$$
最终可以对修改引力重构

---
$f(P)$和
修改成
$$
S=\int \sqrt{-g}d^4x\left[\frac{R}{2k}+f(P)\right]
$$
(m, n)-type Barrow Holographic Dark Energy (BHDE)
$$
L=\frac{1}{a^n(t)}\int_t^\infty a^n(t')dt'
$$
选取$$
a(t)=a_0 t^\delta
$$
$f(\mathcal{Q})$
The Levi-Civita connection
The Weitzenböck connection
引力不通过曲率而是通过仿射连接
$$
	S=\int \sqrt{-g}d^4x\left[\frac{f(\mathcal{Q})}{2k}+\mathcal{L}_m\right]
$$


![[Pasted image 20240906022205.png]]
$$
w_{DE}'=\frac{d}{d \ln a}w_{DE}
$$
![[Pasted image 20240906022229.png]]
$$
r=\frac{\dddot{a}}{aH^3},\ \ s^*=\frac{r-1}{3(q-1/2)}
$$
![[Pasted image 20240906022341.png]]


---
f(R)


在FRW度规下ricci scalar满足以下约束
$$
R=-6\left(\dot{H}+2H^2+\frac{k}{a^2}\right)
$$


$$\frac{1}{2}\left(g_{ab}\left(-f^{(3)}(R)g^{cd}\nabla_c(R)\nabla_d(R)-f''(R)g^{cd}\nabla_d(\nabla_c(R))-f^{(3)}(R)\nabla_c(R)\nabla^c(R)-f''(R)\nabla_c(\nabla^c(R))+f(R)\right)-2f'(R)g_{ac}g_{bd}R^{cd}+2f^{(3)}(R)\nabla_a(R)\nabla_b(R)+f''(R)\nabla_a(\nabla_b(R))+f''(R)\nabla_b(\nabla_a(R))\right)$$


---

修改引力的形式
ref: 修改引力理论与宇宙学（二） - Chauncey的文章 - 知乎
https://zhuanlan.zhihu.com/p/344975864
1. Standard form
   $$\mathcal{L}=\mathcal{L}(g^{\mu \nu})$$
2. Palatini form
3. 'vierbein' Form
4. Plebanski Form


计划：哪些修改引力理论
全息暗能量选择一种
选择一种修改引力，从拉氏量得到场方程，在FRW度规下得到修改后的两个Friedmann方程和连续方程
用这三个方程得到一个微分方程，采用边界条件和初始条件，然后算出它的解（数值解）
画图，和其他暗能量模型的修该引力重构比较（一定要是同一种修改模型）

 $f(Q)$是广义对称引力，Symmetric Teleparallel Gravity，曲率（curvature）和挠率（torsion）都是零，引力的几何性质通过“**非度量性**”（non-metricity）来描述。
 即，度量张量的协变导数不再为零。即
 $$
 Q_{\alpha \mu \nu}=\nabla_\alpha g_{\mu \nu}
$$
作用量变成
$$
S=\int d^4x \sqrt{-g} f(Q)
$$
是一种对称平行的引力（无曲无挠）

$f(T)$是基于 **Teleparallel Gravity**（平行引力理论）的扩展。在平行引力理论中，使用“**扭率**”（torsion）而不是“曲率”（curvature）来描述引力场。
有挠无曲
挠率张量的定义
$$
T^\rho_{\mu \nu}=\Gamma^\rho_{\nu \mu}-\Gamma^\rho_{\mu \nu}
$$
挠率标量
$$
T=\frac{1}{2}T^{\mu \nu}_\rho T^\rho_{\mu \nu}
$$
作用量
$$
S=\int d^4x \sqrt{-g} f(T)
$$

根据全息暗能量重构修改引力
用修改引力的宇宙建立全息暗能量（这个更好）

选择哪两个呢？