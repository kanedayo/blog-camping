# �ݒ��

 bundle install --without production
 bundle exec camping -d .camping.db nuts.rb
 bundle exec rackup config.ru
 heroku create
 git push heroku master
 heroku apps:rename campingtest
 heroku addons:add heroku-postgresql
 heroku pg
 heroku pg:promote HEROKU_POSTGRESQL_ORANGE_URL # DATABASE_URL�̐ݒ�
 heroku config  # �ݒ�̊m�F
 heroku pg:psql # ���[�J����postgreSQL�������Ă����炱���炪�֗��B

