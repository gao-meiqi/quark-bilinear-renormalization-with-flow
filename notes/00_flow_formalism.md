# Gradient Flow Formalism

Gradient flow is a field-theoretical framework that introduces an additional flow-time coordinate $t_f \ge 0$ and evolves quantum fields along this direction according to diffusion-like equations.

Originally proposed by Lüscher, the gradient flow has become a powerful tool in lattice gauge theory. One of its most remarkable properties is that correlation functions of flowed fields at positive flow time possess improved ultraviolet behavior.

This note introduces the basic concepts of the gradient flow formalism, including the definition of flow time, the flow equations, and the interpretation of flowed fields as smeared fields.

---

## Flow Time as an Extra Dimension

在普通 QCD 中，场只依赖于四维时空坐标：

$$
A_\mu(x),
\qquad
\psi(x).
$$

Gradient flow 引入一个新的参数

$$
t_f \ge 0,
$$

称为 **flow time**。

于是场变成

$$
B_\mu(t_f,x),
\qquad
\chi(t_f,x).
$$

其中：

- $x$ 是物理时空坐标；
- $t_f$ 不是物理时间；
- $t_f$ 只是一个辅助演化参数。

因此 gradient flow 常被描述为定义在

$$
\mathbb R^4 \times \mathbb R_+
$$

上的一个五维理论。

需要特别强调的是：

> Flow time 并不是新的物理自由度，而是用于定义 flowed field 的辅助参数。

---

## Diffusion Picture

理解 gradient flow 最简单的方法是热传导方程（diffusion equation）：

$$
\partial_{t_f}\phi(t_f,x)
=
\partial^2\phi(t_f,x).
$$

如果初始条件为

$$
\phi(0,x)
=
\phi_0(x),
$$

则高频模式会随着 flow time 增大而迅速衰减。

在动量空间中，

$$
\phi(t_f,p)
=
e^{-t_f p^2}
\phi(0,p).
$$

因此当

$$
p^2 \gg \frac1{t_f}
$$

时，

$$
e^{-t_f p^2}
\ll 1.
$$

高动量模式会被指数压制。

因此可以把 gradient flow 理解成一种

> UV filter.

或者说是一种连续的 smearing procedure。

---

## Smearing Radius

在树图近似下，

Yang–Mills flow equation 可近似写成

$$
\partial_{t_f} B_\mu
=
\partial^2 B_\mu.
$$

其解为

$$
B_\mu(t_f,x)
=
\int d^4y\,
K_{t_f}(x-y)\,
A_\mu(y),
$$

其中

$$
K_{t_f}(z)
=
\frac{1}{(4\pi t_f)^2}
\exp\left(
-\frac{z^2}{4t_f}
\right)
$$

是热核（heat kernel）。

因此 flowed field 实际上是原始场的高斯平均。

热核的均方宽度为

$$
\sqrt{8t_f}.
$$

因此定义

$$
r_s
=
\sqrt{8t_f},
$$

称为 **smearing radius**。

物理上可以理解为：

> Flowed field 会把半径约为 $\sqrt{8t_f}$ 范围内的信息进行平均。

---

## Why "Gradient" Flow?

名称中的 "gradient" 来自于作用量的梯度下降（gradient descent）。

Yang–Mills 作用量为

$$
S_{\mathrm{YM}}
=
\frac14
\int d^4x\,
G_{\mu\nu}^a
G_{\mu\nu}^a.
$$

对场进行变分，

$$
\frac{\delta S_{\mathrm{YM}}}
     {\delta B_\mu}
=
-
D_\nu G_{\nu\mu}.
$$

因此 Yang–Mills flow equation

$$
\partial_{t_f} B_\mu
=
D_\nu G_{\nu\mu}
$$

可以写成

$$
\partial_{t_f} B_\mu
=
-
\frac{\delta S_{\mathrm{YM}}}
     {\delta B_\mu}.
$$

这与优化问题中的最速下降法完全一致：

$$
\dot{x}
=
-\nabla f(x).
$$

因此这种演化过程被称为

> Gradient Flow.

