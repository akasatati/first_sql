# first_sql
オライリーの「初めてのSQL」の環境構築をdockerで行うもの

# 起動まで
```shell
cp .env.example .env
docker-compose build
docker-compose up -d
```

# 接続を楽をする
```shell
docker-compose exec db bash
mysql -u$MYSQL_USER -p$MYSQL_PASSWORD -P3306 -hdb $MYSQL_DATABASE
```
