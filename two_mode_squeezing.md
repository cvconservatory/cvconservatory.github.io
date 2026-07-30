# Two-mode squeezing
## Definition
The two-mode squeezing gate is defined as

$S_2(t) = \exp\left( t\left[  \hat{a}_1^{\dagger}\hat{a}_2^{\dagger} - \hat{a}_1\hat{a}_2\right]\right) = \exp\left( -i \frac{t}{\hbar} (\hat{q}_1 \hat{p}_2 + \hat{p}_1 \hat{q}_2)\right)$

with Hamiltonian matrix 

$$H =  -t \begin{pmatrix} 0 & 0 & 0 & 1 \\\\ 0 & 0 & 1 & 0 \\\\ 0 & 1 & 0 & 0 \\\\ 1 & 0 & 0 & 0 \end{pmatrix}$$ 

which gives

$$
[q_1 \ p_1 \ q_2 \ p_2] \frac{H}{2 \hbar} \begin{bmatrix} q_1 \\\\ p_1 \\\\ q_2 \\\\ p_2 \end{bmatrix} = -\frac{t}{\hbar} (\hat{q}_1 \hat{p}_2 + \hat{p}_1 \hat{q}_2) 
$$

## Heisenberg Action
In the Heisenberg picture one can write

$$S_2(t)^\dagger \begin{pmatrix}  \hat{q}_1 \\\\ \hat{p}_1 \\\\ \hat{q}_2 \\\\ \hat{p}_2 \end{pmatrix}S_2(t) = e^{-\Omega H} \begin{pmatrix}  \hat{q}_1 \\\\ \hat{p}_1 \\\\ \hat{q}_2 \\\\ \hat{p}_2 \end{pmatrix} = M \begin{pmatrix}  \hat{q}_1 \\\\ \hat{p}_1 \\\\ \hat{q}_2 \\\\ \hat{p}_2 \end{pmatrix}$$

where 

$$M =\begin{pmatrix} \cosh t & 0 & \sinh t & 0 \\\\ 0 & \cosh t & 0 & -\sinh t \\\\ \sinh t & 0 & \cosh t & 0 \\\\ 0 & -\sinh t & 0 & \cosh t \end{pmatrix}.$$ 

The above matrix is already in the Bloch-Messiah and Iwasawa form.

## Decomposition
The two-mode squeezing operation can be decomposed using a 50:50 beam splitter and two single-mode squeezers in Hilbert space

$$S_2(t) = B_{12}(-\pi/4) \left[ S_1(t) \otimes S_1(-t) \right] B_{12}(\pi/4),$$

where $B_{12}(\theta) = \exp\left(\theta (\hat{a}_1^\dagger \hat{a}_2 - \hat{a}_1 \hat{a}_2^\dagger)\right)$ is the beam splitter operator.

## Bargmann Representation
We now compute the coherent-state matrix elements of $S_2(t)$

$$ \exp(\tfrac12 \left[ |\boldsymbol{\alpha}|^2 +  |\boldsymbol{\beta}|^2 \right]) \langle \boldsymbol{\alpha}^* \vert S_2(t) \vert \boldsymbol{\beta} \rangle =  \tfrac{1}{\cosh t} \exp\left[\tfrac12 [\boldsymbol{\alpha}^T \  \boldsymbol{\beta}^T] A \begin{bmatrix} \boldsymbol{\alpha} \\\\ \boldsymbol{\beta} \end{bmatrix} \right] $$

with 

$$A =  \begin{pmatrix} 0 & \tanh t & \text{sech} \ t & 0 \\\\ \tanh t & 0 & 0 & \text{sech} \ t \\\\ \text{sech} \ t & 0 & 0 & -\tanh t \\\\ 0 & \text{sech} \ t & -\tanh t & 0 \end{pmatrix}.$$
