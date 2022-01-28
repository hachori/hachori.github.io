---
layout: single
title:  "Colab에서 파일 업로드하기!"
---

# Colab에서 파일 업로드하기

~~~python
from google.colab import files

uploaded = files.upload()

for fn in uploaded.keys():
  print('User uploaded file "{name}" with length {length} bytes'.format(
      name=fn, length=len(uploaded[fn])))
      
~~~


