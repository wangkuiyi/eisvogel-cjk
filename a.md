---
title: "用 Pandoc 排版包含 LaTeX 公式的汉语 PDF"
subtitle: ""
author: "王益"
titlepage: true,
titlepage-text-color: "000000"
titlepage-rule-color: "360049"
titlepage-rule-height: 0
titlepage-background: "/Users/yi/.local/share/pandoc/templates/cover.png"
---


看到 https://zhuanlan.zhihu.com/p/81704534 这篇文章，发现 Pandoc 竟然有这么好用的一个插件。

试试 LaTeX 公式呢：

\begin{align*}
  f(x) &= x^2\\
  g(x) &= \frac{1}{x}\\
  F(x) &= \int^a_b \frac{1}{3}x^3
\end{align*}
