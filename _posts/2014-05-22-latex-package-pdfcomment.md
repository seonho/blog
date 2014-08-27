---
layout: post
title: LaTex에서 생성할 pdf 문서에 comment 추가하기
comments: true
redirect_from: "2014/05/22/latex-package-pdfcomment/"
permalink: latex-package-pdfcomment
tags: [LaTeX, Package, pdfcomment]
---

[pdfcomment](http://www.ctan.org/pkg/pdfcomment) 패키지는 LaTeX에서 pdf 파일에 annotation과 comment를 추가할 수 있게 해준다.

사용하려면 다음과 같이 하자.

```latex
\usepackage[author={편집자 이름}]{pdfcomment}
% optional
\usepackage[rgb]{xcolor} % color 이름을 사용할 수 있도록 함
```

몇 가지 명령을 소개하면

* \pdfcomment: 현재 위치에 comment 추가.
	- avatar, icon, subject, author, opacity, open 등의 옵션 지정 가능.
* \pdfmarkupcomment: 선택된 영역에 밑줄, 취소선, highlight와 함께 comment를 추가.
	- markup, color를 지정할 수 있다.

사용예

```latex
\pdfmarkupcomment[markup=StrikeOut, color=red]{이 문장은 취소선으로 표시됩니다.}{여기에 comment를 작성합니다.}

\pdfmarkupcomment[markup=Underline, color=red]{이 문장은 밑줄 표시됩니다.}{여기에 comment를 작성합니다.}

\pdfmarkupcomment[markup=Highlight, color=yellow]{이 문장은 highlight로 표시됩니다.}{여기에 comment를 작성합니다.}
```

## 참고

[도은님의 pdfcomment 소개](http://doeun.blogspot.kr/2010/10/latex-package-pdfcomment.html)
