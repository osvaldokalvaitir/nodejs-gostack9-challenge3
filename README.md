# Node - Desafio 3 (Novo)

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/osvaldokalvaitir/node-desafio3-novo/blob/master/LICENSE)
![](https://img.shields.io/github/package-json/v/osvaldokalvaitir/node-desafio3-novo.svg)
![](https://img.shields.io/github/last-commit/osvaldokalvaitir/node-desafio3-novo.svg?color=red)
![](https://img.shields.io/github/languages/top/osvaldokalvaitir/node-desafio3-novo.svg?color=yellow)
![](https://img.shields.io/github/languages/count/osvaldokalvaitir/node-desafio3-novo.svg?color=lightgrey)
![](https://img.shields.io/github/languages/code-size/osvaldokalvaitir/node-desafio3-novo.svg)
![](https://img.shields.io/github/repo-size/osvaldokalvaitir/node-desafio3-novo.svg?color=blueviolet)
[![made-for-VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)](https://code.visualstudio.com/)
![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

Aplicação Meetapp usando Node.js, Express, Multer, date-fns, Mongoose, Bee-Queue, Nodemailer, Express Handlebars, Youch, dotenv, Mailtrap e Sentry.

## Desafio 03. Continuando aplicação

Durante esse desafio vamos aprimorar a aplicação Meetapp que demos início no desafio anterior implementando funcionalidades que aprendemos durante as aulas até agora.

### Funcionalidades

Abaixo estão descritas as funcionalidades que você deve adicionar em sua aplicação.

#### Gerenciamento de arquivos

Crie uma rota para upload de arquivos que cadastra em uma tabela o caminho e nome do arquivo e retorna todos dados do arquivo cadastrado.

#### Gerenciamento de meetups

O usuário pode cadastrar meetups na plataforma com título do meetup, descrição, localização, data e hora e imagem (banner). Todos campos são obrigatórios. Adicione também um campo user_id que armazena o ID do usuário que organiza o evento.

Não deve ser possível cadastrar meetups com datas que já passaram.

O usuário também deve poder editar todos dados de meetups que ainda não aconteceram e que ele é organizador.

Crie uma rota para listar os meetups que são organizados pelo usuário logado.

O usuário deve poder cancelar meetups organizados por ele e que ainda não aconteceram. O cancelamento deve deletar o meetup da base de dados.

#### Inscrição no meetup

O usuário deve poder se inscrever em meetups que não organiza.

O usuário não pode se inscrever em meetups que já aconteceram.

O usuário não pode se inscrever no mesmo meetup duas vezes.

O usuário não pode se inscrever em dois meetups que acontecem no mesmo horário.

Sempre que um usuário se inscrever no meetup, envie um e-mail ao organizador contendo os dados relacionados ao usuário inscrito. O template do e-mail fica por sua conta :)

#### Listagem de meetups

Crie uma rota para listar os meetups com filtro por data (não por hora), os resultados dessa listagem devem vir paginados em 10 itens por página. Abaixo tem um exemplo de chamada para a rota de listagem dos meetups:

```
http://localhost:3333/meetups?date=2019-07-01&page=2
```

Nesse exemplo, listaremos a página 2 dos meetups que acontecerão no dia 01 de Julho.

Nessa listagem retorne também os dados do organizador.

#### Listagem de inscrições

Crie uma rota para listar os meetups em que o usuário logado está inscrito.

Liste apenas meetups que ainda não passaram e ordene meetups mais próximos como primeiros da lista.

## Índice

- [Desenvolvimento](#desenvolvimento)

  - [Configuração do Ambiente](#configuração-do-ambiente)

  - [Instalação do Projeto](#instalação-do-projeto)

  - [Configuração das Variáveis de Ambiente](#configuração-das-variáveis-de-ambiente)

  - [Execução do Projeto](#execução-do-projeto)

  - [Execução do Ouvinte de Fila](#execução-do-ouvinte-de-fila)

- [Utilizados no Projeto](#utilizados-no-projeto)

  - [Bibliotecas](#bibliotecas)

  - [APIs](#apis)

  - [Ferramentas](#ferramentas)

## Desenvolvimento

### Configuração do Ambiente

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/README.md) e siga `Configuração de Ambiente`.

### Instalação do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Instalação de Projeto`.

### Configuração das Variáveis de Ambiente

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/dotenv.md) e siga `Configuração de Variáveis de Ambiente`.

### Execução do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Execução de Projeto para Desenvolvimento` ou `Execução de Projeto para Produção`.

### Execução do Ouvinte de Fila

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/bee-queue.md) e siga `Execução de Ouvinte de Fila`.

## Utilizados no Projeto

### Bibliotecas

- [@sentry/node](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@sentry-node.md)

- [bcrypt.js](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/bcryptjs.md)

- [Bee-Queue](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/bee-queue.md)

- [date-fns](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/date-fns.md)

- [dotenv](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/dotenv.md)

- [ESLint](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint.md)

- [eslint-config-prettier](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint-config-prettier.md)

- [eslint-plugin-prettier](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint-plugin-prettier.md)

- [Express](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express.md)

- [Express Handlebars](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express-handlebars.md)

- [Express Handlebars plugin for Nodemailer](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemailer-express-handlebars.md)

- [ExpressJS Async Errors](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express-async-errors.md)

- [Json Web Token](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/jsonwebtoken.md)

- [Mongoose](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/mongoose.md)

- [Multer](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/multer.md)

- [Nodemailer](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemailer.md)

- [Nodemon](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemon.md)

- [pg](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/pg.md)

- [pg-hstore](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/pg-hstore.md)

- [Prettier](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/prettier.md)

- [Sequelize](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/sequelize.md)

- [sequelize-cli](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/sequelize-cli.md)

- [Sucrase](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/sucrase.md)

- [Youch](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/youch.md)

- [Yup](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/yup.md)

### APIs

- **Interna**

  - **Rotas**

    - Meetups

      - Lista todas as meetups de uma data ou não
      - Adiciona novas meetups
      - Edita dados de meetups existentes
      - Exclui meetups existentes

    - Inscrições

      - Lista todas as meetups que um usuário está inscrito
      - Adiciona novas inscrições

    - Organizando

      - Lista todas as meetups que um usuário está organizando

    - Usuários

      - Adiciona novos usuários
      - Edita dados de usuários existentes

    - Sessões

      - Adiciona novas sessões

    - Arquivos

      - Adiciona novos arquivos

### Ferramentas

- [Docker](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/docker.md)

  - Imagem do MongoDB: [mongo](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/mongo.md)

  - Imagem do PostgreSQL: [postgres](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/postgres.md)

  - Imagem do Redis: [redis:alpine](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/redis-alpine.md)

- [Insomnia](https://github.com/osvaldokalvaitir/projects-settings/blob/master/api/insomnia.md)

- [Mailtrap](https://github.com/osvaldokalvaitir/projects-settings/blob/master/email/mailtrap.md)

- [MongoDB Compass Community](https://github.com/osvaldokalvaitir/projects-settings/blob/master/database/mongodb/mongodb-compass-community.md)

- [Postbird](https://github.com/osvaldokalvaitir/projects-settings/blob/master/database/postgresql/postbird.md)

- [Sentry](https://github.com/osvaldokalvaitir/projects-settings/blob/master/error/sentry.md)
