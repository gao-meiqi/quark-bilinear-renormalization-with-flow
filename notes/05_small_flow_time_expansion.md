# Small Flow-Time Expansion

The small flow-time expansion (SFTE) provides a systematic connection between flowed operators and local operators in the original quantum field theory.

For sufficiently small flow time, a flowed operator can be expanded as

$$
\mathcal O(t,x)
=
\sum_i c_i(t)\,\mathcal O_i(x),
$$

where the coefficients $c_i(t)$ can be calculated perturbatively.

This framework plays a central role in extracting renormalized operators from flowed observables and serves as the theoretical foundation of many gradient-flow applications.

The purpose of this note is to introduce the general idea of the small flow-time expansion and its derivation.

### Flow-time version of the OPE
Small Flow-Time Expansion is a flow-time version of the OPE.

### Why does the SFTE coefficient not contain $Z_\chi$
When first reading the literature on the small flow-time expansion (SFTE), one may wonder why the matching coefficient is usually written as
$$
\tilde{O}(t_f)=ζ_O​(μ,t_f)O_R​(μ)+O(t_f)
$$
instead of 
$$
O(t_f)=Z_χ^{−1}​ζ_O​(μ,t_f)O_R​(μ)+O(t_f)=ζ'_O​(μ,t_f)O_R​(μ)+O(t_f)
$$
After all, flowed fermion fields require an additional renormalization factor $Z_\chi$.

ANS:

Since the factor $Z_\chi$ is universal, it is independent of the choice of bilinear structure Γ.
Therefore it is convenient to absorb $Z_\chi$ into the definition of the flowed fermion field itself.

从费曼图看更直观
$χˉ​Γχ$ 的一圈修正结果通常长成 $$1+16π2g2​(A_{ext}​+A_{vertex}​).$$
$Z_\chi$ 吸收 $A_{ext}$ 只剩下 $A_{vertex}$, 于是 matching coefficient 只需要处理 operator structure $A_{vertex}$.

---

A.

\[
\zeta_O \approx Z_O
\]

B.

**\(t\to0\) , flowed operator 与 local operator 的对应关系**

> The coefficient \(\zeta_O\) is not ONLY a renormalization constant of the flowed fermion field. It is a matching coefficient between a finite flowed operator and a renormalized local operator.

> *$\zeta_O$ is a matching coefficient whose perturbative structure contains the renormalization information of the local operator $O_R$.
In particular, the anomalous dimension associated with $Z_O$ reappears in the logarithmic flow-time dependence of $\zeta_O$.*

---
> **field renormalization**、**operator renormalization** 和 **SFTE matching** 这三个层次是理解 flow renormalization 的关键。

The following three concepts should be clearly distinguished:

1. Field renormalization

$$
\chi_R = Z_\chi^{-1/2}\chi
$$

This removes UV divergences associated with flowed fermion fields.

2. Operator renormalization

$$
O_R = Z_O^{-1}O_B
$$

This removes UV divergences associated with composite operator insertions.

3. SFTE matching

$$
\widetilde O(t)
=
\zeta_O(\mu,t) O_R(\mu)
+
O(t)
$$

This relates a finite flowed operator to a renormalized local operator in the small flow-time limit.