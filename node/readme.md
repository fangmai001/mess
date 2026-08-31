# node

### 獲取
docker pull node:22-alpine

### 打包tag
docker save -o node_22-alpine.tar node:22-alpine

### 載入
docker load -i node_22-alpine.tar

### 校驗 (md5)
63cdef337fc3215662e3249dded80ed0  node_22-alpine.tar
