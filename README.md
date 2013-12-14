# 設定例

 bundle install --without production
 bundle exec camping -d .camping.db nuts.rb
 bundle exec rackup config.ru
 heroku create
 git push heroku master
 heroku apps:rename campingtest
 heroku addons:add heroku-postgresql
 heroku pg
 heroku pg:promote HEROKU_POSTGRESQL_ORANGE_URL # DATABASE_URLの設定
 heroku config  # 設定の確認
 heroku pg:psql # ローカルにpostgreSQLが入っていたらこちらが便利。

