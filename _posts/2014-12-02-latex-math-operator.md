---
layout: post
title: LaTeX math operators and functions
comments: true
redirect_from: "2014/12/02/latex-math-operator/"
permalink: latex-math-operator
tags: [LaTeX, Math, Operator]
---

자주 사용하는 operator와 함수를 정리해둔다.

```latex
% Define argmin and argmax operators
\DeclareMathOperator*{\argmin}{\arg\!\min}
\DeclareMathOperator*{\argmax}{\arg\!\max}

% Define trace operator
\DeclareMathOperator*{\trace}{Tr}

% Define expectation operator
\DeclareMathOperator*{\expect}{E}

% Define variance operator
\DeclareMathOperator{\var}{var}

% Define covariance operator
\DeclareMathOperator{\cov}{cov}

% Define signum function operator
\DeclareMathOperator{\sgn}{sgn}

%\newcommand{\covariance}[1]{\operatorname{cov} \left( #1 \right)}
%\newcommand{\expectation}[1]{\operatorname{E} \left[ #1 \right]}
```

참고

[vert vs. mid](http://tex.stackexchange.com/questions/498/mid-vertical-bar-vert-lvert-rvert-divides)
