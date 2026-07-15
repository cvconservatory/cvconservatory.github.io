# Cubic phase gate
The cubic phase gate is defined as

$``P(t) = \exp\left( i t \hat{q}^2 / 2 \hbar \right)``$

with Hamiltonian matrix $`` \begin{pmatrix} t & 0 \\ 0 & 0 \end{pmatrix}``$. 

In the Heisenberg picture one can write

$``P(s)^\dagger \begin{pmatrix}  \hat{q} \\ \hat{p} \end{pmatrix}P(s) = e^{-\Omega H} \begin{pmatrix}  \hat{q} \\ \hat{p} \end{pmatrix} = S \begin{pmatrix}  \hat{q} \\ \hat{p} \end{pmatrix}``$

where $``S =\begin{pmatrix} 1 & 0 \\ t & 1 \end{pmatrix} ``$. The above matrix has the Bloch-Messiah decomposition

$``S =  R(\theta) [e^r \oplus e^{-r}] R(\theta - \tfrac{\pi}{2}), \ R(\theta) =
 \begin{pmatrix}
	\cos \theta &-\sin \theta \\
	\sin \theta & \cos \theta
\end{pmatrix},   ``$

where the parameters above are related to $t\geq0$ as follows  $\sinh r = t/2, \  \theta = \tan^{-1} e^{r}$.

The above equations gives rise to the following decomposition in Hilbert space

$``P(t) = e^{i \varphi}\exp\left( i \theta \hat{a}^\dagger \hat{a} \right) \exp(\tfrac{r}{2}(\hat{a}^{\dagger 2} - \hat{a}^2)) \exp\left( i (\theta - \tfrac{\pi}{2}) \hat{a}^\dagger \hat{a}  \right) ``$

where $``\exp(i \varphi) = \frac{\sqrt[4]{1+\tfrac{t^2}{4}} }{\sqrt{1 - i \tfrac{t}{2}}}``$.

We now compute the coherent-state matrix elements of $P(t)$

$$\langle \alpha^* \vert P(t) \vert \beta \rangle = \langle \alpha^* \vert e^{i \varphi}\exp\left( i \theta \hat{a}^\dagger \hat{a} \right) \exp(\tfrac{r}{2}(\hat{a}^{\dagger 2} - \hat{a}^2)) \exp\left( i (\theta - \tfrac{\pi}{2}) \hat{a}^\dagger \hat{a}  \right) \vert \beta \rangle,$$

where we use the following identity to express the squeezing operator as 

$$\exp{\left(\frac{r}{2}(\hat{a}^{\dagger 2} - \hat{a}^{2})\right)} = \exp{\left(\frac{\tanh{r}}{2}\hat{a}^{\dagger 2}\right)}\exp{\left(-[\hat{a}^{\dagger}\hat{a} + 1/2]\ln{\cosh{r}}\right)}\exp{\left(-\frac{\tanh{r}}{2}\hat{a}^{2}\right)},$$

and a second identity to normal-order this expression

$$\exp{(\theta \hat{a}^{\dagger}\hat{a})} = :\exp{([\exp{(\theta)} - 1]\hat{a}^{\dagger}\hat{a})}:,$$

with $:(\hat{a}^{\dagger}\hat{a})^{p}: = \hat{a}^{\dagger p}\hat{a}^{p}$.

Using these two identities, the decomposition of $P(t)$ takes the form

$$P(t) = e^{i\varphi} \exp(i\theta \hat{a}^{\dagger}\hat{a})\exp{\left(\frac{\tanh{r}}{2}\hat{a}^{\dagger 2}\right)}\times:\frac{\exp{([1/\cosh{r}-1]\hat{a}^{\dagger}\hat{a})}}{\sqrt{\cosh{r}}}:\times\exp{\left(-\frac{\tanh{r}}{2}\hat{a}^{2}\right)}\exp{(i(\theta - \tfrac{\pi}{2})\hat{a}^{\dagger}\hat{a})}.$$

Evaluating the matrix element $\langle \alpha^* \vert \dots \vert \beta \rangle = e^{i\varphi} \langle \bar{\alpha}^* \vert \dots \vert \bar{\beta} \rangle$ gives

$$e^{i\varphi} \langle \bar{\alpha}^* \vert \exp{\left(\frac{\tanh{r}}{2}\hat{a}^{\dagger 2}\right)}\times:\frac{\exp{([1/\cosh{r}-1]\hat{a}^{\dagger}\hat{a})}}{\sqrt{\cosh{r}}}:\times\exp{\left(-\frac{\tanh{r}}{2}\hat{a}^{2}\right)} \vert \bar{\beta} \rangle,$$

where we have introduced the rotated labels $\langle \bar{\alpha}^* \vert \equiv \langle \alpha^* e^{-i\theta} \vert = \langle \alpha^* \vert e^{i\theta \hat{a}^{\dagger}\hat{a}}$ and $\vert \bar{\beta} \rangle \equiv \vert \beta e^{i(\theta - \tfrac{\pi}{2})} \rangle = e^{i(\theta - \tfrac{\pi}{2}) \hat{a}^{\dagger}\hat{a}} \vert \beta \rangle$ to simplify the expression. The resulting expression takes the form

$$\sqrt{2}e^{i\varphi} \frac{\exp{[-\frac{1}{2}(\lvert \alpha \rvert^{2} + \lvert \beta \rvert^{2})]}}{\sqrt[4]{4+t^{2}}} \exp{\left(-\frac{1}{2} \begin{bmatrix} \alpha & \beta \end{bmatrix} \begin{bmatrix} f & f-1 \\\\ f-1 & f \end{bmatrix} \begin{bmatrix} \alpha \\\\ \beta \end{bmatrix} \right)},$$

where we used the overlap of two coherent states $\langle \bar{\alpha}^* \vert \bar{\beta} \rangle = \exp{(-\frac{1}{2}(\lvert\alpha\rvert^{2} + \lvert\beta\rvert^{2} - 2\bar{\alpha}\bar{\beta}))}$, and the function $f$ is given in terms of the parameter $t$ by

$$
f = \frac{t}{2i+t}.
$$

An important result is

$$
[\hat{a},P(t)] = P\left\lbrace \frac{it}{2}(\hat{a}^{\dagger} + \hat{a}) \right\rbrace.
$$

We calculate the Fock-state matrix elements of the commutator above

$$
\langle m|[\hat{a},P(t)]|n \rangle = \sqrt{m+1}\,P_{m+1,n} - \sqrt{n}\,P_{m,n-1} = \frac{it}{2}\left\lbrace \sqrt{n+1}\,P_{m,n+1} + \sqrt{n}\,P_{m,n-1} \right\rbrace,
$$

with the initial condition $P_{0,0} = \frac{e^{i\varphi}}{\sqrt{\cosh{r}}} = \frac{1}{\sqrt{1 - it/2}}$.

The other recurrence relations are

$$
P_{m+1,n} = \frac{1}{\sqrt{m+1}}\left\lbrace -\sqrt{m}P_{m-1,n}f -\sqrt{n}P_{m,n-1}(f-1) \right\rbrace,
$$

$$
P_{m,n+1} = \frac{1}{\sqrt{n+1}}\left\lbrace -\sqrt{m}P_{m-1,n}(f-1) - \sqrt{n}P_{m,n-1}f \right\rbrace,
$$

with the same initial value $P_{0,0}$.