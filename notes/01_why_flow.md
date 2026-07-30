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


### 廖老师先问了flow 是干嘛的
- 我说了半天 然后 消除紫外发散 而且我解释了为什么可以消除紫外发散 从kernel和半径

### 廖老师说 lattice本身就消除了发散 为什么又来一个消除发散 而且还要在lattice上用
### 然后老师说格点本身就比连续好
### 现在又引入连续 反而又能做重整化 逻辑??

- 我回答了 lattice确实消除了这个发散 但是有限的东西还是要进一步重整化 (想到有点跑题) 再加入gradient flow的因素 我说的是 把粗的格子 细的格子 给变成一个能标 (其实!! almost 后面说 更大的半径 统一的动量 clean计算 会不会好一些??) (但是这样好像也只是解释 HOW) (如果捋顺逻辑的话 我会回答什么呢0.0) (好像我的课题本身 也不是从 flow的优势出发 它只是其中的一个方法 最大的[mixing]优势太远0.0) (或者回答 转到某个能标后进行微扰计算这个系数 但是但是 老师似乎又是考虑的 更大的视角 是lattice理论本身的性质(可能是认为有限已经是很好的按道理不需要再涉及任何连续 但是又用连续很奇怪)) ()

### 梁老师救援: 没有强调什么能标跑动而是强调scheme本身 但是大概的意思也是 格点本身的量需要到msbar [不过好像也还是没有回答 关于为什么要 离散-引入连续的东西-重整化]

### 所以廖老师后面又问了这个flow方案的年份

### 廖老师后来指出了一个typo

### 梁老师问了我this work的图 有没有外推?? pion怎么样了??


- 虽然感觉当时大脑根本就转不起来 以为很糟糕的回答 但是 重新情景复现竟然觉得还可以0.0





