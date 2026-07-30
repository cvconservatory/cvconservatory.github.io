# Pauli, Hadamard and Cayley Matrices

Everyone is familiar with the Pauli matrices

$$
\sigma_1 = X=\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}, \quad  \sigma_2 = Y=\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}, \quad \sigma_3=Z=\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}.
$$

They satisfy all sort of nice properties such as $\sigma_i \sigma_j = \delta_{i j} \sigma_0 + i \epsilon_{ijk}\sigma_k$, $[\sigma_j, \sigma_k] = 2 i \epsilon_{jkl}\sigma_l$ and $\{\sigma_j, \sigma_k\} = 2 \delta_{jk} \sigma_0$ with $\sigma_0$ the $2 \times 2$ identity matrix.

We will also introduce the (real) symplectic matrix

$$
\Omega  = i  Y = \begin{pmatrix} 0 & 1 \\ -1 & 0
\end{pmatrix}.
$$

It is also well-known that the Hadamard matrix 

$$
H = \tfrac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix},
$$
 
allows us to write $H X H=  Z$ and that it connects the eigenbases of $X$ and $Z$

$$
Z \ket{i} = (-1)^{i} \ket{i}, i \in \{0,1\},\quad 
X \ket{\pm} = \pm \ket{\pm}, \text{then }, \quad 
\ket{+} = H \ket{0} \text{ and } \ket{-} = H \ket{1}.
$$

It is not that often noted that we can also construct a similar matrix connecting $Z$ and $Y$. This matrix is called the Cayley matrix

$$
\Gamma = \tfrac{1}{\sqrt{2}} \begin{pmatrix} 1 & -i \\ 1 & i \end{pmatrix}
$$

which gives $\Gamma Y \Gamma^\dagger = Z$. One can also define $R = \Gamma^*$ and obtain $R Y R^\dagger  = - Z$. Thus if we call $\ket{i \pm}$ to be the eigenkets of $Y$, satisfying $Y \ket{\pm i} = \pm \ket{\pm i}$ then

$$
\ket{i+} = \Gamma^\dagger \ket{0} \text{ and } \ket{i-} = \Gamma^\dagger \ket{1}
$$ 

They also satisfy $\Gamma \Gamma^T = R R^T = X$, i.e., they both give a Takagi-Autonne decomposition of $X$. Moroever, $\Gamma Z \Gamma^\dagger = X$  which implies that we can write

$$
\ket{+} = \Gamma \ket{0}, \quad \ket{-} = i \Gamma \ket{1}.
$$

Note that when $\Gamma$ acts on a real-valued vector it produces a vector in which the second entry is the complex conjugate of the first one

$$
\Gamma \begin{pmatrix} q \\ p \end{pmatrix} = \tfrac{1}{\sqrt{2}} \begin{pmatrix} 1 & -i \\ 1 & i \end{pmatrix} \begin{pmatrix} q \\ p \end{pmatrix} = \tfrac{1}{\sqrt{2}} \begin{pmatrix} q -i p \\ q+ i p\end{pmatrix} = \tfrac{1}{\sqrt{2}} \begin{pmatrix} \alpha^* \\ \alpha\end{pmatrix}, \quad \alpha := q+i p . 
$$