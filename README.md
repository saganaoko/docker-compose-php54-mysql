# PHP5.4 Dcoker Compose
CentOS7 x PHP5.4の環境です。mysqlはおまけです。

## Instlation
```
git clone git@github.com:saganaoko/docker-compose-php54-mysql.git
cd docker-compose-php54-mysql
cp .env.example .env
// 環境に合わせて.envの内容を変更してください
cp php/conf.d/sample.conf.example hogehoge.conf
// 環境に合わせてconfの内容を変更してください
docker-compose build
docker-compose up -d
// localhost:8081でアクセスしてください
```
