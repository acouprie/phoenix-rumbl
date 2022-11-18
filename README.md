# Phoenix v1.5.3 (Elixir) with Docker

This is a new ready to use Phoenix v1.5.3 (Elixir) project including a Postgresql database with Docker.

## Requirements

- Docker
- Docker Compose

## Usage

```bash
$ mix deps.get
$ docker-compose up
```

### Prepare the DB

```bash
$ docker-compose run --rm phoenix mix ecto.create
$ docker-compose run --rm phoenix mix ecto.migrate
```

### Install node modules

```bash
$ cd src/assets
$ npm install
```

### Access the app

Get http://localhost:4000

## Acknowledgements

Insprired by [Dockerizing a Phoenix and Elixir Application](https://medium.com/swlh/use-docker-to-create-an-elixir-phoenix-development-environment-e1a81def1d2e), but fixing some issues caused by Python and Node version.
