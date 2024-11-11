suppose we input a $1\times n$ vector $\boldsymbol{x_i}$
linear transformations
$$
z_{i+1}=x_iW_{i+1}+b_{i+1}
$$
其中$x_i$是输入的$1\times n$向量，$W_{i+1}$是$n \times m$矩阵$m$表示隐藏层的神经元，$b_{i+1}$表示bias
nonlinear function
$$
x_{i+1}=f(z_{i+1})
$$
where activation function $f$ usually use ELU, relu,  sigmod, tanh etc.
So we can get output vector $\hat{y}$ and $y$ is initially input data equally to $\boldsymbol{x_0}$
$$
\hat{y}=x_{i+1}v_{i+2}+s_{i+2}
$$
where $v_{i+2}$ denote $1\times m$ vector is a map between hidden layer and output layer
Loss function is defined by
$$
Loss=(y-\hat{y})^2
$$
we need to make loss function to be minimal
$$
\min \sum_{i=1}^N Loss_i
$$
