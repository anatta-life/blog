# 整除

## 定义

给定整数 $a$, $b$, 且$a \ne 0$, 若$\exists m \in \mathbb{Z}$ s.t. $b=ma$, 则成$b$是$a$的`倍数`, 或者$a$`整除`$b$, 并记为$a \mid b$, 也称为$a$
是 $b$ 的 `因子/约数/除数`, 否则称$a$`不整除`$b$, 并记为$a \nmid b$

注意
- 遇到$a \mid b$或$a \nmid b$, 均认为$a \ne 0$
- 整除的定义用$ax = b$的可解性

## 性质

对整数$a, b, c$

- $a \mid a$
- $a \mid b$且$b \ne 0$, 则: $|b| > |a|$
- 若$a \mid b$且$b \mid a$, 则$b = \pm a$
- 若$a \mid b$且$b \mid c$, 则$a \mid c$
- 若$a \mid b$且$a \mid c$, 则$\forall x,y \in Z$都有$a \mid bx + cy$.
- 若$c \ne 0$, 则$a \mid b \Leftrightarrow ac \mid bc$

## 判定(带余除法)
给定两个正整数$a, b$, 那么$\exists_1$的一对整数$q, r$满足
$b = a q + r$ 且 $0 \le r < a$.

注意
- 称$q$为$b$除以$a$的商, $r$为$b$除以$a$的余数.
- 为啥带余除法是对的?

证明

- 存在性:
  - 已知: $a, b \in \mathbb{N}$
  - 未知: $\exists q, r \in \mathbb{Z}$ s.t. $b = aq + r$, $0 \le r < a$
  - 联系
    - 难点在哪?: $0 \le r < a$
    - $r = ?$: $r = b - aq \Rightarrow 0 \le b - aq < a \Rightarrow \frac{b}{a}-1 < q \le\frac{b}{a} \Rightarrow \lfloor \frac{b}{a} \rfloor$
- 唯一性
