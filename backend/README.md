<h1 align="center">
    <img alt="GoBarber" src="./src/assets/logo-purple.svg" width="200px" />
</h1>

<h3 align="center">
  GoBarber - API desenvolvida em NodeJS
</h3>

<h3 align="center">
  #rocketseat, #nodejs, #express, #sequelize, #mongodb, #redis, #jwt, #nodemailer, #youch, #yup
</h3>

<p align="center">
  <a href="#gobarber-sobre-a-aplicação">Sobre a Aplicação</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#gobarber-como-rodar">Como rodar</a>
</p>


## :gobarber-sobre-a-aplicação: Sobre a Aplicação

A aplicação desenvolvida é um gerenciador de agendamentos de uma barbearia, o **GoBarber**. Essa aplicação consiste em um API em NodeJs que tem por finalidade cadastrar usuários/prestadores de serviços e realizar agendamentos.

Abaixo segue todas as tecnologias que foram abordadas no desenvolvimento da aplicação.

## Tecnologias utilizadas no back-end do GoBarber
- NodeJs
- Express
- Sucrase
- MongoDB
- Mongoose
- Sequelize
_ Docker
- Redis
- Postgresql
- Nodemailer
- Multer
- Yup
- Youch
- Sentry
- Bee-queue

## Como rodar

#### para a utilização dos bancos, o arquivo de environment (.env) deve ser preenchido.

### Iniciando containeres do docker com os bancos de dados

Caso já possua os containeres, basta apenas starta-los

```bash
$ docker start NOME_DO_CONTAINER
```

#### PostgreSQL

```bash
$ docker run --name db_postgres -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
```

#### MongoDB
```bash
$ docker run --name mongobarber -p 27017:27017 -d -t mongo
```

#### Redis

```bash
docker run --name redisbarber -p 6379:6379 -d -t redis:alpine
```

## Aplicação em Nodejs

Basta ter um gerenciador de pacotes do node instaldo (yarn / npm), para instalar as dependencias do package.json, dentro da pasta root

```bash
$ yarn
```

```bash
$ npm install
```

Para iniciar a aplicação

```bash
$ yarn dev
```

Para rodar a fila utilizando Redis

```bash
$ yarn queue
```

