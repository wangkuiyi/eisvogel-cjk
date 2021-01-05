作者：fri3nd
链接：https://zhuanlan.zhihu.com/p/81704534
来源：知乎
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

---
title: "如何使用 pandoc 和 latex 制作漂亮的 pdf"
subtitle: ""
author: [Tuya.Inc]
date: "2019-09-08"
header-left: "/Users/fri3nds/.pandoc/templates/tuya-logo.png"
titlepage: true,
titlepage-text-color: "000000"
titlepage-rule-color: "360049"
titlepage-rule-height: 0
titlepage-background: "/Users/yi/.local/share/pandoc/templates/cover.png"
---


## 1. 前言

markdown 是很多程序员都喜爱的文档格式，简洁切功能强大，通过一些 markdown 文本编辑器可以方便导出成 pdf 文件，但是不同的 markdown 支持的主题导出的 pdf 差别还是很大，很
多现代编译器在编辑过程中，并不能很好地发现 ‘零宽度字符’, 导致出现了一些很难发现的 bug。即使是这样 markdown 还是我的最爱，快速且方便，随便文本编辑器都可以打开，也可以看懂，
只是没有 preview 的功能。

但是有一些需要输出到其他格式文件时，markdown 就有点显得不太够用。这个时候就需要我们今天的主角之一的 `pandoc`

## 2. 文本转换工具 Pandoc

[pandoc](https://pandoc.org/) 是用 haskell 编写的一个 cli 工具，可以支持 docx、epub、html、json、latex、markdow、vimwiki、org、asciidoc 等等格式之间互相转
换。mac、windows、linux 的安装也都是很简单，官方都有安装教程。

## 3. 文本编排工具 LaTeX/TeX

LaTeX，是一种基于 TeX 的排版系统。 TeX 是由美国计算机 Donald Ervin Knuth 编写的排版软件。至于 Donald Ervin Knuth 真的是神人。Donald Ervin Knuth 编写 TeX 的原
因，就是当时计算机的排版技术十分粗糙，影响到他的巨著《计算机程序设计艺术》的印刷质量，老爷子就决定自己编写一个排版软件：TeX。

用 word 写过毕业论文的都知道，word 的排版真的不是很好用，很多人应该都是用不好的，word 也有自己的宏什么的，掌握很好的话，使用起来也是很方便的，但是很多时候，鼠标的误操作
就导致文本携带的编排细心丢失，而且还有各种版本的问题。至少没有什么人用 word 来编排书籍吧。但是 LaTeX 就可以很好的胜任（为什么我们学校毕业论文没有 LaTeX 模板啊，很多期刊
论文都是用自己的 LaTex 模板啊）。
