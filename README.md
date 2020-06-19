# rails_docker_env

docker-composeで立てるDocker Rails MySQLの環境ファイルです。手順は
１.このフォルダをクローン
２.
docker-compose.ymlの
```
environment:     
      MYSQL_ROOT_PASSWORD: banana
```
このbananaは各自ルートパスワードを入力。

3.ターミナルで
```
$ docker-compose run web rails new . --force --database=mysql --skip-bundle
```

4.config/database.ymlを下のように変更

