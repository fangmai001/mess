# python

### 獲取
docker pull python:3.12-slim

### 打包tag
docker save -o python_3.12-slim.tar python:3.12-slim

### 載入
docker load -i python_3.12-slim.tar

### 校驗 (md5)
15417c5ed8070b57d63c8c47b6116e52  python_3.12-slim.tar
