# Anomalous Dimension

In classical field theory, the scaling behavior of an operator is determined by its canonical dimension.

Quantum corrections modify this scaling behavior.

The difference between the quantum scaling dimension and the canonical dimension is called the anomalous dimension.

Anomalous dimensions play a central role in renormalization, renormalization-group evolution, and the small flow-time expansion.

The purpose of this note is to introduce the basic idea of anomalous dimensions and explain why they naturally appear in gradient-flow calculations.

### Canonical Dimension

Consider the quark field

$$
\psi(x).
$$

From the QCD action,

$$
\bar\psi i\!\not\!\!D\psi,
$$

one finds

$$
[\psi]
=
\frac32.
$$

Therefore

$$
[\bar\psi\psi]
=
3.
$$

Similarly,

$$
[\bar\psi\gamma_\mu\psi]
=
3.
$$

These are called canonical dimensions.

### Quantum Corrections

After quantization, loop corrections introduce logarithmic dependence on the renormalization scale μ.

As a result, operators no longer scale exactly according to their canonical dimensions.

Instead,

$$
O_R(\mu)
=
Z_O^{-1}(\mu) O_B.
$$

The renormalization factor $Z_O$ depends on μ.

Therefore the operator itself becomes scale dependent.

### Definition of the Anomalous Dimension

The anomalous dimension is defined by

$$
\gamma_O(\mu)
=
-
\mu
\frac{d}{d\mu}
\ln Z_O.
$$

Equivalently,

$$
\mu
\frac{d}{d\mu}
O_R(\mu)
=
-\gamma_O(\mu)
O_R(\mu).
$$

This equation describes how the operator changes when the renormalization scale is varied.

### Physical Interpretation

The anomalous dimension measures how much quantum fluctuations modify the scaling behavior of an operator.

Classically,

$$
O(x)
\sim
\lambda^{-d}.
$$

Quantum mechanically,

$$
O(x)
\sim
\lambda^{-d-\gamma}.
$$

Therefore the anomalous dimension represents a purely quantum effect.

If no quantum correction exists,

$$
\gamma=0.
$$

> Example: Conserved Vector Current

For the conserved vector current,

$$
V_\mu
=
\bar\psi\gamma_\mu\psi,
$$

current conservation implies

$$
Z_V=1.
$$

Therefore

$$
\gamma_V=0.
$$

The vector current does not run with μ.

> Example: Scalar Density

The scalar density

$$
S
=
\bar\psi\psi
$$

requires renormalization,

$$
S_R
=
Z_S^{-1}S_B.
$$

Its anomalous dimension is nonzero.

Consequently,

$$
S_R(\mu)
$$

depends on the renormalization scale.

This is closely related to the running of the quark mass.


### Why It Appears in the SFTE

Consider the small flow-time expansion

$$
\widetilde O(t)
=
\zeta_O(\mu,t)
O_R(\mu)
+
O(t).
$$

> bare quantity!!

Applying

$$
\mu\frac{d}{d\mu}
$$

gives

$$
\left(
\mu\frac{\partial}{\partial\mu}
+
\gamma_O
\right)
\zeta_O
=
0.
$$

Thus the matching coefficient must compensate for the anomalous dimension of the local operator.

This is why logarithms such as

$$
\ln(\mu^2 t)
$$

naturally appear in SFTE calculations.

*竟然还有这一层 0.0??*


>  $\zeta_V$ and the error estimate:
> $$
> \gamma_V=0,
> $$
> 因此 matching coefficient
> $$
> \zeta_V
> $$
> 在精确理论中应该与重整化尺度 μ 无关。
>
> 实际计算只做到有限阶，所以会残留少量 μ dependence。
>
> 这种 dependence 并不是物理效应，而是高阶项尚未计算导致的。
>
> 因此人们通常通过改变 μ 来估计 perturbative uncertainty。
>
> 如果从 NLO 到 NNLO 曲线越来越平，说明微扰展开正在收敛。