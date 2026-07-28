# LaTeX, Vector Calculus & Matrices Cheatsheet

## LaTeX Basics

### Text Formatting
- `\textbf{text}` → **bold**
- `\textit{text}` → *italic*
- `\underline{text}` → underline
- `\texttt{text}` → monospace

### Greek Letters
- `\alpha` → $\alpha$
- `\beta` → $\beta$
- `\gamma` → $\gamma$
- `\delta` → $\delta$
- `\theta` → $\theta$
- `\lambda` → $\lambda$
- `\mu` → $\mu$
- `\pi` → $\pi$
- `\sigma` → $\sigma$
- `\omega` → $\omega$

### Mathematical Operators
- `\sum` → $\sum$
- `\prod` → $\prod$
- `\int` → $\int$
- `\oint` → $\oint$
- `\partial` → $\partial$
- `\nabla` → $\nabla$
- `\infty` → $\infty$
- `\pm` → $\pm$
- `\times` → $\times$\nabla \times \mathbf{E} = -\frac{\partial \mathbf{B}}{\partial t
- `\cdot` → $\cdot$

### Fractions & Roots
- `\frac{a}{b}` → $\frac{a}{b}$
- `\sqrt{x}` → $\sqrt{x}$
- `\sqrt[n]{x}` → $\sqrt[n]{x}$

### Superscripts & Subscripts
- `x^2` → $x^2$
- `x_i` → $x_i$
- `x^{2n+1}` → $x^{2n+1}$
- `x_{i,j}` → $x_{i,j}$

### Brackets & Delimiters
- `(` `)` → parentheses
- `[` `]` → square brackets
- `\{` `\}` → curly braces
- `\lvert` `\rvert` → $\lvert x \rvert$ (absolute value)
- `\lVert` `\rVert` → $\lVert v \rVert$ (norm)

---

## Vector Calculus

### Vectors
- Vector notation: $\mathbf{v}$ or $\vec{v}$ 
  - LaTeX: `\mathbf{v}` or `\vec{v}`
  - Components: $\mathbf{v} = \langle v_1, v_2, v_3 \rangle$

### Dot Product (Scalar Product)
$$\mathbf{u} \cdot \mathbf{v} = u_1v_1 + u_2v_2 + u_3v_3$$

Alternative: `\mathbf{u} \cdot \mathbf{v}` or `\langle \mathbf{u}, \mathbf{v} \rangle`

### Cross Product
$$\mathbf{u} \times \mathbf{v} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{vmatrix}$$

### Gradient (∇)
$$\nabla f = \left\langle \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \right\rangle$$

LaTeX: `\nabla f` or `\nabla \mathbf{F}`

### Divergence
$$\nabla \cdot \mathbf{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y} + \frac{\partial F_z}{\partial z}$$

LaTeX: `\nabla \cdot \mathbf{F}`

### Curl
$$\nabla \times \mathbf{F} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ F_x & F_y & F_z \end{vmatrix}$$

LaTeX: `\nabla \times \mathbf{F}`

### Laplacian
$$\nabla^2 f = \Delta f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2}$$

LaTeX: `\nabla^2 f` or `\Delta f`

### Line Integral
$$\int_C \mathbf{F} \cdot d\mathbf{r}$$

### Surface Integral
$$\iint_S \mathbf{F} \cdot d\mathbf{S}$$

### Volume Integral
$$\iiint_V f \, dV$$

---

## Matrices

### Basic Matrix Notation
$$\mathbf{A} = \begin{pmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{pmatrix}$$

LaTeX environments:
- `pmatrix` → parentheses $()$
- `bmatrix` → square brackets $[]$
- `Bmatrix` → curly braces $\{\}$
- `vmatrix` → determinant bars $||$
- `Vmatrix` → double bars

### Matrix Operations

#### Transpose
$$\mathbf{A}^T \text{ or } \mathbf{A}'$$

LaTeX: `\mathbf{A}^T` or `\mathbf{A}^{\top}`

#### Inverse
$$\mathbf{A}^{-1}$$

LaTeX: `\mathbf{A}^{-1}`

#### Determinant
$$\det(\mathbf{A}) \text{ or } |\mathbf{A}|$$

LaTeX: `\det(\mathbf{A})` or `|\mathbf{A}|`

#### Trace
$$\text{tr}(\mathbf{A}) = a_{11} + a_{22} + \cdots + a_{nn}$$

LaTeX: `\text{tr}(\mathbf{A})`

### Matrix Multiplication
$$(\mathbf{A}\mathbf{B})_{ij} = \sum_{k=1}^{n} a_{ik}b_{kj}$$

### Eigenvalues & Eigenvectors
$$\mathbf{A}\mathbf{v} = \lambda \mathbf{v}$$

Characteristic equation:
$$\det(\mathbf{A} - \lambda \mathbf{I}) = 0$$

### Common Matrices

#### Identity Matrix
$$\mathbf{I} = \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$$

#### Zero Matrix
$$\mathbf{0} = \begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}$$

#### Diagonal Matrix
$$\mathbf{D} = \begin{pmatrix} d_1 & 0 & 0 \\ 0 & d_2 & 0 \\ 0 & 0 & d_3 \end{pmatrix}$$

### Matrix Properties
- Symmetric: $\mathbf{A} = \mathbf{A}^T$
- Orthogonal: $\mathbf{A}^T\mathbf{A} = \mathbf{I}$
- Singular: $\det(\mathbf{A}) = 0$ (no inverse)
- Non-singular: $\det(\mathbf{A}) \neq 0$ (has inverse)

### Solving Linear Systems
$$\mathbf{A}\mathbf{x} = \mathbf{b}$$
$$\mathbf{x} = \mathbf{A}^{-1}\mathbf{b}$$

---

## Useful Combinations

### Gradient Vector
$$\nabla \mathbf{F} = \begin{pmatrix} \frac{\partial F}{\partial x} \\ \frac{\partial F}{\partial y} \\ \frac{\partial F}{\partial z} \end{pmatrix}$$

### Jacobian Matrix
$$\mathbf{J} = \begin{pmatrix} \frac{\partial f_1}{\partial x_1} & \cdots & \frac{\partial f_1}{\partial x_n} \\ \vdots & \ddots & \vdots \\ \frac{\partial f_m}{\partial x_1} & \cdots & \frac{\partial f_m}{\partial x_n} \end{pmatrix}$$

### Hessian Matrix
$$\mathbf{H} = \begin{pmatrix} \frac{\partial^2 f}{\partial x^2} & \frac{\partial^2 f}{\partial x \partial y} \\ \frac{\partial^2 f}{\partial y \partial x} & \frac{\partial^2 f}{\partial y^2} \end{pmatrix}$$
