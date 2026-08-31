# postgres

### 獲取
docker pull postgres:16-alpine

### 打包tag
docker save -o postgres_16-alpine.tar postgres:16-alpine

### 分割檔案
split -b 50M -d postgres_16-alpine.tar postgres_16-alpine.tar.part_

### 合併檔案
cat postgres_16-alpine.tar.part_* > postgres_16-alpine.tar

### 載入
docker load -i postgres_16-alpine.tar

### 校驗 (md5)
2fcde909a8343af7244dda73d6e1e387  postgres_16-alpine.tar
