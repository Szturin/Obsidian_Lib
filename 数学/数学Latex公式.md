---
tags:
  - 数学/考研数学
  - obsidian/obsidian入门
aliases:
topic:
date:
type:
---

$$
\begin{vmatrix}a & b\\
c & d
\end{vmatrix}=ad-bc
$$


---
title: 学术笔记模板
date: 2025-12-23
tags: [学术, LaTeX, 模板]
---

# [课题名称]

> [!info] 笔记说明
> 本笔记使用 LaTeX 增强排版。行内公式使用 `$公式$`，块级公式使用 `$$公式$$`。

---

## 1. 核心定义 (Definition)
**术语名称**：在此输入术语的中文描述。

$$
\text{定义：} \mathcal{D} \subseteq \mathbb{R}^n \implies \forall \epsilon > 0, \exists \delta > 0
$$
> [!tip] 技巧
> 使用 `\mathcal` 可以打出花体字母，常用于表示集合或空间。

---

## 2. 定理与推导 (Theorem & Derivation)

### 2.1 定理内容
$$
\boxed{ \int_{a}^{b} f(x) dx = F(b) - F(a) } \tag{1.1}
$$

### 2.2 证明过程
使用 `aligned` 环境可以让等号对齐，这是最常用的排版方式：

$$
\begin{aligned}
\text{证明：} & \text{ 设 } \Phi(x) = \int_{a}^{x} f(t) dt \\
& \because \Phi'(x) = f(x) \quad \text{(根据微积分基本定理)} \\
& \therefore \Phi(x) = F(x) + C \\
& \text{当 } x = a \text{ 时，} \Phi(a) = 0 \implies C = -F(a) \\
& \text{故：} \Phi(b) = F(b) - F(a) \quad \square
\end{aligned}
$$

---

## 3. 复杂结构展示

### 3.1 矩阵排版

可以使用 `array` 环境实现带分割线的矩阵：

$$
\mathbf{M} = \left[
\begin{array}{cc|c}
1 & 0 & \mu \\
0 & 1 & \sigma \\
\hline
0 & 0 & 1
\end{array}
\right]
$$

### 3.2 分段函数
$$
f(x) = 
\begin{cases} 
\frac{1}{x} & \text{if } x \neq 0 \\
0 & \text{if } x = 0 
\end{cases}
$$

---

## 4. 延伸思考
- [[相关