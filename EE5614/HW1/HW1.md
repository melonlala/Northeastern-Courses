# Problem 1
### (a)
$$
\begin{aligned}
E[X] &= \sum_x p(x)x \\
	&= -2\cdot\frac{3}{8} - 1\cdot\frac{1}{8} + 0 + 1\cdot\frac{1}{4} \\
	&= -\frac{5}{8} 
\end{aligned}
$$

$$
\begin{aligned}
E[X^2] &= \sum_x p(x)x^2 \\
&= 4\cdot\frac{3}{8} + 1\cdot\frac{1}{8} + 0 + 1\cdot\frac{1}{4} \\
	  &= \frac{15}{8}
\end{aligned}
$$



### (b) 
$$
\begin{aligned}
\mathrm{Var}[Y] &= \mathrm{Var}[3X+1] = 9\mathrm{Var}[X] \\
&=9\left(E[X^2] - (E[X])^2\right) \\
&=9\left(\tfrac{15}{8} - \left(-\tfrac{5}{8}\right)^2\right) \\
&=9\left(\tfrac{15}{8} - \tfrac{25}{64}\right) \\
&=9\cdot\tfrac{95}{64} = \tfrac{855}{64} 
\end{aligned}
$$

# Problem 2

### (a)

$$
P = 
\begin{pmatrix}
0.4 & 0 & 0.6 \\
0.7 & 0.1 & 0.2 \\
0.3 & 0.5 & 0.2
\end{pmatrix}
$$

### (b)
$
p(x_k = c | x_{k-1} =a) = P_{1, 3} = 0.6 $



$
p(x_k = c | x_{k-2} =a)  = (P \cdot P)_{1, 3} = 0.6 * 0.4 + 0.2 * 0 + 0.2 * 0.6 = 0.36
$

In the Markov chain, the probability of current state $x_k$ only depends on the last state. The two-step probability accounts for all possible paths through intermediate states, while the one-step probability is a direct transition.


# Problem 3

### (a)
$Q^*(a^1) = E(R(a^1)) = 0.6$

$Q^*(a^2) = E(R(a^2)) = 0.5$

$\pi^* = a^1$


### (b)

$Q(a^1)_1 = 0 + 0.6*0.2 = 0.12$

$Q(a^2)_2 = 0 + 0.6 * 0.9 = 0.54$

$Q(a^1)_3 = 0.12 + 0.6*(0-0.12) = 0.048$

$Q(a^1)_4 = 0.048 + 0.6*(1.3-0.048) = 0.7992$

$Q(a^2)_5 = 0.54 + 0.6(0.1-0.54) = 0.276$

So $Q(a^1) = 0.7992, Q(a^2) = 0.276$

### (c)
$$
\begin{aligned}
&Q(a^1)_1=5+0.6(0.2−5)=5+0.6(−4.8)=2.12  \\

&Q(a^2)_2=5+0.6(0.9−5)=5+0.6(−4.1)=2.54 \\

&Q(a^1)_3=2.12+0.6(0−2.12)=0.848 \\

&Q(a^1)_4=0.848+0.6(1.3−0.848)=1.1192 \\

&Q(a^2)_5=2.54+0.6(0.1−2.54)=1.076
\end{aligned}
$$

So $Q(a^1) = 1.1192, Q(a^2) = 1.076$


### (d)

$ P(a^2) = 0.15, P(a^1) = 0.85$


# Problem 4
$$
\begin{aligned}
&\pi_1(a^1) = \pi_1(a^2) = 0.5 \\
&H_2(a^1) = 0 + 0.6 \times (0-0)(1-0.5) = 0 \\
&H_2(a^2) = 0 - 0.6 \times (0-0)(0.5) = 0 \\
&\pi_2(a^1) = \pi_2(a^2) = 0.5 \\
&H_3(a^1) = 0 + 0.6 \times \left(1-0.5\right)(1-0.5) = 0.3 \\
&H_3(a^2) = 0 - 0.6 \times \left(1-0.5\right) \times 0.5 = -0.3 \\
&\pi_3(a^1) = \frac{e^{0.3}}{e^{0.3} + e^{-0.3}} \approx 0.6457 \\
&\pi_3(a^2) = 1 - 0.6457 = 0.3543 \\
&H_4(a^2) = -0.3 + 0.6(0.5-0.5)(1-\pi_3(a^2)) = -0.3 \\
&H_4(a^1) = 0.3 - 0.6(0.5-0.5) \times \pi_3(a^2) = 0.3 \\
&\pi_4(a^1) = \frac{e^{0.3}}{e^{0.3} + e^{-0.3}} \approx 0.6457 \\
&\pi_4(a^2) = 1 - 0.6457 = 0.3543
\end{aligned}
$$



# Problem 1

### (a)

$$
\begin{aligned}
E[X] &= \sum_x p(x) \cdot x \\
&= (-2) \cdot \frac{3}{8} + (-1) \cdot \frac{1}{8} + 0 \cdot \frac{1}{4} + 1 \cdot \frac{1}{4} \\
&= -\frac{6}{8} - \frac{1}{8} + 0 + \frac{2}{8} \\
&= -\frac{5}{8}
\end{aligned}
$$

$$
\begin{aligned}
E[X^2] &= \sum_x p(x) \cdot x^2 \\
&= 4 \cdot \frac{3}{8} + 1 \cdot \frac{1}{8} + 0 \cdot \frac{1}{4} + 1 \cdot \frac{1}{4} \\
&= \frac{12}{8} + \frac{1}{8} + 0 + \frac{2}{8} \\
&= \frac{15}{8}
\end{aligned}
$$

### (b)

$$
\begin{aligned}
\mathrm{Var}[Y] &= \mathrm{Var}[3X + 1] = 9 \cdot \mathrm{Var}[X] \\
&= 9 \left( E[X^2] - (E[X])^2 \right) \\
&= 9 \left( \frac{15}{8} - \left( -\frac{5}{8} \right)^2 \right) \\
&= 9 \left( \frac{15}{8} - \frac{25}{64} \right) \\
&= 9 \left( \frac{120}{64} - \frac{25}{64} \right) \\
&= 9 \cdot \frac{95}{64} \\
&= \frac{855}{64}
\end{aligned}
$$

---

# Problem 2

### (a)

$$
P = 
\begin{pmatrix}
0.4 & 0 & 0.6 \\
0.7 & 0.1 & 0.2 \\
0.3 & 0.5 & 0.2
\end{pmatrix}
$$

### (b)

$$
p(x_k = c \mid x_{k-1} = a) = P_{1,3} = 0.6
$$

$$
\begin{aligned}
p(x_k = c \mid x_{k-2} = a) &= (P^2)_{1,3} \\
&= P_{1,1} \cdot P_{1,3} + P_{1,2} \cdot P_{2,3} + P_{1,3} \cdot P_{3,3} \\
&= 0.4 \times 0.6 + 0 \times 0.2 + 0.6 \times 0.2 \\
&= 0.24 + 0 + 0.12 \\
&= 0.36
\end{aligned}
$$

**Explanation:** In a Markov chain, the probability of the current state $x_k$ depends only on the immediately preceding state $x_{k-1}$ (the Markov property). The two-step probability accounts for all possible paths through intermediate states, while the one-step probability is a direct transition.

---

# Problem 3

### (a)

$$
\begin{aligned}
&Q^*(a^1) = E[R(a^1)] = \mu = 0.6 \\
&Q^*(a^2) = E[R(a^2)] = \frac{-0.2 + 1.2}{2} = 0.5 \\
&\pi^* = \arg\max_a Q^*(a) = a^1
\end{aligned}
$$

### (b)

Initialize $Q(a^1) = Q(a^2) = 0$, with $\alpha = 0.6$:

$$
\begin{aligned}
&Q_1(a^1) = 0 + 0.6 \times (0.2 - 0) = 0.12 \\
&Q_2(a^2) = 0 + 0.6 \times (0.9 - 0) = 0.54 \\
&Q_3(a^1) = 0.12 + 0.6 \times (0 - 0.12) = 0.048 \\
&Q_4(a^1) = 0.048 + 0.6 \times (1.3 - 0.048) = 0.7992 \\
&Q_5(a^2) = 0.54 + 0.6 \times (0.1 - 0.54) = 0.276
\end{aligned}
$$

**Final:** $Q(a^1) = 0.7992$, $Q(a^2) = 0.276$, $\pi = a^1$

### (c)

Initialize $Q(a^1) = Q(a^2) = 5$ (optimistic), with $\alpha = 0.6$:

$$
\begin{aligned}
&Q_1(a^1) = 5 + 0.6 \times (0.2 - 5) = 5 - 2.88 = 2.12 \\
&Q_2(a^2) = 5 + 0.6 \times (0.9 - 5) = 5 - 2.46 = 2.54 \\
&Q_3(a^1) = 2.12 + 0.6 \times (0 - 2.12) = 0.848 \\
&Q_4(a^1) = 0.848 + 0.6 \times (1.3 - 0.848) = 1.1192 \\
&Q_5(a^2) = 2.54 + 0.6 \times (0.1 - 2.54) = 1.076
\end{aligned}
$$

**Final:** $Q(a^1) = 1.1192$, $Q(a^2) = 1.076$, $\pi = a^1$

### (d)

Using $\varepsilon$-greedy with $\varepsilon = 0.3$ and $|A| = 2$:

$$
\begin{aligned}
&\pi(a^1) = 1 - \varepsilon + \frac{\varepsilon}{|A|} = 1 - 0.3 + \frac{0.3}{2} = 0.85 \\
&\pi(a^2) = \frac{\varepsilon}{|A|} = \frac{0.3}{2} = 0.15
\end{aligned}
$$

---

# Problem 4

Initialize $H_1(a^1) = H_1(a^2) = 0$, with $\alpha = 0.6$.

**k = 1:** Action $a^1$, Reward $r_1 = 0$, Baseline $\bar{r}_1 = 0$

$$
\begin{aligned}
&\pi_1(a^1) = \pi_1(a^2) = 0.5 \\
&H_2(a^1) = 0 + 0.6 \times (0 - 0)(1 - 0.5) = 0 \\
&H_2(a^2) = 0 - 0.6 \times (0 - 0) \times 0.5 = 0
\end{aligned}
$$

**k = 2:** Action $a^1$, Reward $r_2 = 1$, Baseline $\bar{r}_2 = 0$

$$
\begin{aligned}
&\pi_2(a^1) = \pi_2(a^2) = 0.5 \\
&H_3(a^1) = 0 + 0.6 \times (1 - 0)(1 - 0.5) = 0.3 \\
&H_3(a^2) = 0 - 0.6 \times (1 - 0) \times 0.5 = -0.3
\end{aligned}
$$

**k = 3:** Action $a^2$, Reward $r_3 = 0.5$, Baseline $\bar{r}_3 = \frac{0 + 1}{2} = 0.5$

$$
\begin{aligned}
&\pi_3(a^1) = \frac{e^{0.3}}{e^{0.3} + e^{-0.3}} \approx 0.6457 \\
&\pi_3(a^2) = 1 - 0.6457 = 0.3543 \\
&H_4(a^2) = -0.3 + 0.6 \times (0.5 - 0.5)(1 - 0.3543) = -0.3 \\
&H_4(a^1) = 0.3 - 0.6 \times (0.5 - 0.5) \times 0.6457 = 0.3
\end{aligned}
$$

**Final Answers:**

$$
\begin{aligned}
&H_4(a^1) = 0.3, \quad H_4(a^2) = -0.3 \\
&\pi_4(a^1) = \frac{e^{0.3}}{e^{0.3} + e^{-0.3}} \approx 0.6457 \\
&\pi_4(a^2) = 1 - 0.6457 = 0.3543
\end{aligned}
$$

