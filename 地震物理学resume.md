# 地震物理学
## 1 Mechanics of elasticity
### 1.1 Strain
Strain $\epsilon$ is defined as below

$$
\epsilon \equiv \dfrac{u}{L}\quad(u~::~\text{displacement})
$$

Strain tensor is defined as below

$$
\epsilon_{ij}\equiv\dfrac{1}{2}\left(\dfrac{\partial u_i}{\partial x_j}+\dfrac{\partial u_j}{\partial x_i}\right)
$$

Rotation tensor is defined as below 

$$
\omega_{ij}\equiv\dfrac{1}{2}\left(\dfrac{\partial u_i}{\partial x_j}-\dfrac{\partial u_j}{\partial x_i}\right)
$$

Volmetric strain and Deviatoric strain are below

$$
\begin{cases}
tr(\epsilon_{ij})=\epsilon_{ii}=\nabla\cdot \mathbf{u}\\
\epsilon_{ij}' = \epsilon_{ij}-\dfrac{\delta_{ij}\epsilon_{kk}}{3}
\end{cases}
$$

### 1.2 Stress
Traction continuous is below

$$
\mathbf{T(n)}=-\mathbf{T(-n)}
$$

The relation below traction and Stress tensor is below

$$
\begin{cases}
\mathbf{T_i(n)}=sigma_{ij}n_j\\
\mathbf{T}=\mathbf{\sigma\cdot n}
\end{cases}
$$

テンソル不変量まとめ

$$
\begin{cases}
I_1 = \text{tr}(\sigma) = \sigma_{ii} \\
I_2 = 
\begin{vmatrix}
\sigma_{22} & \sigma_{23} \\
\sigma_{32} & \sigma_{33}
\end{vmatrix} +
\begin{vmatrix}
\sigma_{33} & \sigma_{31} \\
\sigma_{13} & \sigma_{11}
\end{vmatrix} +
\begin{vmatrix}
\sigma_{11} & \sigma_{12} \\
\sigma_{21} & \sigma_{22}
\end{vmatrix} \\
I_3 = \det(\sigma)
\end{cases}
$$

The relation between Stress tensor and Strain tensor is below

$$
\sigma_{ij}=C_{ijkl}\epsilon{ij}
$$

Elastic enegry is below 

$$
e = \dfrac{1}{2}\sigma_{ij}\epsilon_{ij}
$$

In case of Isotoropic material, $C_{ijkl}$ is below

$$
\begin{pmatrix}
\sigma_{11} \\
\sigma_{22} \\
\sigma_{33} \\
\sigma_{12} \\
\sigma_{13} \\
\sigma_{23}
\end{pmatrix} = 
\begin{pmatrix}
\lambda + 2\mu & \lambda & \lambda & 0 & 0 & 0 \\
\lambda & \lambda + 2\mu & \lambda & 0 & 0 & 0 \\
\lambda & \lambda & \lambda + 2\mu & 0 & 0 & 0 \\
0 & 0 & 0 & \mu & 0 & 0 \\
0 & 0 & 0 & 0 & \mu & 0 \\
0 & 0 & 0 & 0 & 0 & \mu
\end{pmatrix}
\begin{pmatrix}
\epsilon_{11} \\
\epsilon_{22} \\
\epsilon_{33} \\
2\epsilon_{12} \\
2\epsilon_{13} \\
2\epsilon_{23}
\end{pmatrix}
$$

Elastic constants are below

$$
\begin{cases}
\kappa = \dfrac{3\lambda + 2\mu}{3}\quad(\text{bulk modulus})\\
E = \dfrac{\mu(3\lambda+2\mu)}{\lambda+\mu}\quad(\text{Young modulus})\\
\nu = \dfrac{\lambda}{2(\lambda+\mu)}\quad(\text{Poisson's ratio})
\end{cases}
$$

Equation of motion of elastic medium is below

$$
\rho\dfrac{\partial^2 \mathbf{u}}{\partial t^2} = \nabla\cdot\mathbf{\sigma}+\mathbf{f}
$$
$$
\rho\dfrac{\partial^2 u_i}{\partial t^2}= \dfrac{\partial \sigma_{ij}}{\partial x_j}+f_i
$$

これまでの式をまとめるとNavier's equationが得られる

$$
\rho\ddot{u}_i=(\lambda+\mu)u_{j,ji}+\mu u_{i,jj}+f_i
$$
$$
\dfrac{\partial^2 \mathbf{u}}{\partial t^2} = \alpha^2\nabla(\nabla\cdot\mathbf{u})-\beta^2\nabla\times\nabla\times\mathbf{u}+\dfrac{\mathbf{f}}{\rho}
$$

Here, $\alpha,~\beta$ is define as below

$$
\begin{cases}
\alpha = \sqrt{\dfrac{\lambda + 2\mu}{\rho}}\quad(\text{P=velocity})\\
\beta = \sqrt{\dfrac{\mu}{\rho}}\quad(\text{S-velocity})
\end{cases}
$$

## 2 Representation theorem and Green's function
***更新中***

