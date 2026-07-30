# Single-mode squeezing
## Definition
The single mode squeezing gate is defined as

$S(t) = \exp\left( \tfrac12 t\left[  a^{\dagger 2} -a^2\right]\right) = \exp\left( -i \frac{t}{2\hbar} (\hat{q} \hat{p} + \hat{p} \hat{q})\right)$

with Hamiltonian matrix 

$$H =  -t \begin{pmatrix} 0 & 1 \\\\ 1 & 0 \end{pmatrix}$$ 

which gives

$$
[q \ p] \frac{H}{2 \hbar} \begin{bmatrix} q \\\\ p \end{bmatrix} = -\frac{t}{2\hbar} (\hat{q} \hat{p} + \hat{p} \hat{q}) 
$$

## Heisenberg Action
In the Heisenberg picture one can write

$$S(t)^\dagger \begin{pmatrix}  \hat{q} \\\\ \hat{p} \end{pmatrix}S(s) = e^{-\Omega H} \begin{pmatrix}  \hat{q} \\\\ \hat{p} \end{pmatrix} = M \begin{pmatrix}  \hat{q} \\\\ \hat{p} \end{pmatrix}$$

where 

$$M =\begin{pmatrix} e^{t} & 0 \\\\ 0 & e^{-t} \end{pmatrix}.$$ 

The above matrix is already in the Bloch-Messiah and Iwasawa form.

## Bargmann Representation
We can compute the coherent-state matrix elements of $S(t)$

$$ \exp(\tfrac12 \left[ |\alpha|^2 +  |\beta|^2 \right]) \langle \alpha^* \vert S(t) \vert \beta \rangle =  \tfrac{1}{\sqrt{\cosh r}} \exp\left[\tfrac12 [\alpha \  \beta] A \begin{bmatrix} \alpha \\\\ \beta \end{bmatrix} \right] $$

with 

$$A =  \begin{pmatrix} \tanh t & \text{sech} \ t  \\\\ \text{sech} \ t & -\tanh t\end{pmatrix}.$$
