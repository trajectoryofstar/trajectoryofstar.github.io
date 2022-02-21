---
layout: post
title: OS in python 
date: 2022-02-22 00:35:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Seoul]
---

```python
import os
import os.path

```

1. import OS 
OS module은 Operating System의 약자로  
운영체제에서 제공되는 여러 기능을 파이썬에서 수행할 수 있게 해줌.

ex) 
1. 파일 복사 - 리눅스 cp
2. 디렉토리 생성 - 리눅스 mkdir 
3. 특정 디렉토리 내의 파일 목록 - 리눅스 ls 

2. os.getcwd()
- 현재 주소 불러옴.

3. os.listdir()
- 현재 존재하는 파일 목록 호출 

```python
for x in os.listdir(os.getcwd()):
    if x.endswith('ipynb'):
        print(x)
```

문법 -> endswith(끝나는문자, 문자열의 시작, 문자열의 끝) 

{% gist trajectoryofstar/5cb94643834afc563d5d6be1de2161d1 %}
