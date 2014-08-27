---
layout: post
title: MEX compile error&#58; unknown type name 'char16_t'
comments: true
redirect_from: "2014/08/14/mex-compile-error-unknown-type-name-char16_t/"
permalink: mex-compile-error-unknown-type-name-char16_t
tags: [MATLAB, mex, char16_t, compile, error]
---

아래와 같은 오류가 나온다면

```matlab
In file included from /Applications/MATLAB_R2013a.app/extern/include/mex.h:58:
In file included from /Applications/MATLAB_R2013a.app/extern/include/matrix.h:294:
/Applications/MATLAB_R2013a.app/extern/include/tmwtypes.h:819:9: error: unknown type name 'char16_t'
typedef char16_t CHAR16_T;
```

다음과 같이 하자.

```
cd /Applications/MATLAB_R2013a.app/bin
system('cp mexopts.sh mexopts.org.sh')
edit mexopts.sh
```

CXXFLAGS를 찾아서 끝부분에 `-std=c++11`을 추가한다.

저장 후, `mex -setup`을 수행한다.

## Reference
- [Stack Overflow](http://stackoverflow.com/questions/22367516/mex-compile-error-unknown-type-name-char16-t)
