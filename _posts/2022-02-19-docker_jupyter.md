---
layout: single
title:  "Dockekr에서 jupyter notebook 바로 실행하기"
---

# 실행 명령어

~~~python
sudo docker run --runtime=nvidia -p 8888:8888 --rm -it hachori:hachori-dl bash -c "export LD_LIBRARY_PATH=/usr/local/cuda/lib64; jupyter notebook --notebook-dir=/home --ip='*' --port=8888 --allow-root"
~~~
