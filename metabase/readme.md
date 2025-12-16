# metabase

### 獲取
docker pull metabase/metabase

### 打包tag
docker save -o metabase_latest.tar metabase/metabase:latest

### 分割檔案
split -b 95M -d metabase_latest.tar metabase_latest.tar.part_

### 合併檔案
cat metabase_latest.tar.part_0* > metabase_latest.tar


