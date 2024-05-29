- 单参微分同胚群：映射$\phi:\mathbb{R}\times M \rightarrow M$组成单参微分同胚群，满足
1. $\phi_t:M \rightarrow M$是微分同胚$\forall t \in \mathbb{R}$
2. $\psi_t \circ \phi_s=\psi_{t+s}, \forall t,s \in \mathbb{R}$
>其作为一个群，恒元是$\phi_0$，群乘法是复合映射，群元是$\phi_t$，群元的集合是$\{ \phi_t| t \in \mathbb{R} \}$

- 张量的对称部分和反称部分，以(0,2)阶张量为例子$$T_{(ab)}\coloneqq \frac{1}{2}(T_{ab}+T_{ba})$$ $$T_{[ab]}\coloneqq \frac{1}{2}(T_{ab}-T_{ba})$$
> 全反称和全对称表示张量只包含有反称部分或对称部分
- Killing矢量场：$(M, g_{ab})$上的矢量场$\xi^a$，若满足其给出的单参微分同胚群$\phi$是单参等度规群。
- 满足Killing方程也是充要条件$$\nabla_a\xi_b+\nabla_b\xi_a=0$$
> Killing矢量场表现了空间的对称性