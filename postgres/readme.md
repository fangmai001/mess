# postgres

### 獲取
docker pull postgres:latest

### 打包tag
docker save -o postgres_latest.tar postgres:latest

### 分割檔案
split -b 95M -d postgres_latest.tar postgres_latest.tar.part_

### 合併檔案
cat postgres_latest.tar.part_0* > postgres_latest.tar


