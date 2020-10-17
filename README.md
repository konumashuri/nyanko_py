# 猫の写真をひたすら写すサービス

# command

- run command
    - `docker-compose run web {some command}`

- start server
    - `docker-compose up`

- create application
    - `docker-compose run web python manage.py startapp {application name}`

- create database
    - `docker-compose run web python manage.py migrate`

- run migration
    - `docker-compose run web python manage.py makemigrations polls`

- 3 steps to change models
    - モデルを変更する (models.py の中の)
    - これらの変更のためのマイグレーションを作成するために `python manage.py makemigrations` を実行します。
    - データベースにこれらの変更を適用するために `python manage.py migrate` を実行します。

- run into console
    - `docker-compose run web python manage.py shell`

- create admin user
    - `docker-compose run web python manage.py createsuperuser`
