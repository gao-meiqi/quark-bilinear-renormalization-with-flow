# Why Gradient Flow?

- The gradient flow was not introduced merely as a mathematical curiosity. Its development was motivated by several long-standing difficulties in quantum field theory and lattice gauge theory, particularly those associated with ultraviolet fluctuations, renormalization, and the construction of composite operators.

- The purpose of this note is to explain the physical motivations behind the gradient flow and why it has become an important tool in modern lattice QCD.

### UV Problem

The ultraviolet divergences originate from quantum fluctuations at arbitrarily short distances. In a lattice simulation these fluctuations are particularly severe because neighboring lattice sites may exhibit large statistical noise.

$x→y, ⟨A(x)A(y)⟩→∞.$

$ψ(x)ψ(x)$*所以不止是因为all to all, 还有物理的原因？*

### The Difficulty of Composite Operators

$\bar{\psi}​Γ\psi$ and ...

more complex due to:
- mixing
- power divergence
- scheme dependence

### The Idea of Smearing

This idea is analogous to image processing. A noisy image can be smoothed by averaging neighboring pixels. Similarly, a quantum field can be smoothed by averaging over nearby spacetime points.

### Why Not Use Arbitrary Smearing

- 平滑
- gauge covariant
- 可系统研究重整化





