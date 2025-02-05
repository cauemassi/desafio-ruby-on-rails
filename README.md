# Desafio Ruby on Rails - README

## [[Changelog]](/CHANGELOG.md)

## [Desenvolvimento]

### Requerimentos

- Ruby 3.3.7
- Redis 4.0
- Postgres 15.5
- Rails 8.0.1

### Setup Inicial

- Instalar Postgres
  ```shell
    $ sudo apt install postgresql postgresql-contrib
    $ sudo -i -u postgres
    $
    $ psql
    $ create role desafio_ruby_on_rails with createdb login password 'desafio_ruby_on_rails';
    $ \q
    $ exit
    $
    $ sudo apt-get install libpq-dev
  ```
- Instalar Ruby
  ```shell
    $ \curl -sSL https://get.rvm.io | bash -s stable
    $ echo 'source "/etc/profile.d/rvm.sh"' >> ~/.bashrc
    $ rvm install 3.3.7
    $ rvm use 3.3.7 --default
  ```
  ```
- Instalar Bundler
  ```shell
    gem bundle install
  ```
- Executar bundle install
  ```bash
    bundle install
  ```
- Executar setup do banco de dados
  ```bash
    rails db:setup  db:seed
  ```
