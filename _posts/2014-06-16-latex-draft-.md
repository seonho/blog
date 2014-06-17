---
layout: post
title: LaTeX에서 draft 문서 표시하기
comments: true
redirect_from: "2014/06/16/latex-package-draftwatermark/"
permalink: latex-package-draftwatermark
tags: [LaTeX, Package, draftwatermark]
---

[draftwatermark](http://www.ctan.org/tex-archive/macros/latex/contrib/draftwatermark) 패키지는 LaTeX에서 draft watermark를 추가할 수 있게 해준다.

아래와 같이 사용하면 되겠다.

```latex
\usepackage{draftwatermark}
\SetWatermarkAngle{45}
\SetWatermarkText{DRAFT}
```
