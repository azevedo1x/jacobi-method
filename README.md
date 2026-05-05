## Linear System Analysis

### Original System
$$
\begin{cases} 
10x + 2y + z = 7 \\ 
x + 5y + z = -8 \\ 
2x + 3y + 10z = 6 
\end{cases}
$$

### Initial Estimates
*   $x_0 = 0.5$
*   $y_0 = -1$
*   $z_0 = 0.5$

---

## Isolation of Variables
To solve using an iterative method (like Jacobi), we isolate the elements of the **main diagonal**:

$$
\begin{aligned}
x &= \frac{1}{10}(7 - 2y - z) \\
y &= \frac{1}{5}(-8 - x - z) \\
z &= \frac{1}{10}(6 - 3y - 2x)
\end{aligned}
$$

---

## Iteration 1 Calculations
Substituting the initial estimates $(x_0, y_0, z_0)$ into the isolated equations:

### Calculating $x_1$
$$x_1 = \frac{1}{10}(7 - 2(-1) - 0.5)$$
$$x_1 = \frac{8.5}{10} = \mathbf{0.85}$$

### Calculating $y_1$
$$y_1 = \frac{1}{5}(-8 - 0.5 - 0.5)$$
$$y_1 = \frac{-9}{5} = \mathbf{-1.8}$$

### Calculating $z_1$
$$z_1 = \frac{1}{10}(6 - 3(-1) - 2(0.5))$$
$$z_1 = \frac{8}{10} = \mathbf{0.8}$$

---

### Results Summary (First Iteration)
> **New Estimates:**  
> $x_1 = 0.85$  
> $y_1 = -1.8$  
> $z_1 = 0.8$
