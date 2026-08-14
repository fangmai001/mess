# gitlab-ee

### 獲取
docker pull gitlab/gitlab-ee:19.2.2-ee.0

### 打包tag
docker save -o gitlab-ee_19.2.2-ee.0.tar gitlab/gitlab-ee:19.2.2-ee.0

### 分割檔案
split -b 50M -d gitlab-ee_19.2.2-ee.0.tar gitlab-ee_19.2.2-ee.0.tar.part_

### 合併檔案
cat gitlab-ee_19.2.2-ee.0.tar.part_* > gitlab-ee_19.2.2-ee.0.tar

### 載入
docker load -i gitlab-ee_19.2.2-ee.0.tar

### 校驗 (md5)
cf9516cd23d6dd0f710d073ce16bba9d  gitlab-ee_19.2.2-ee.0.tar
