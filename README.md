# Node - Desafio 2 (Novo)

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/osvaldokalvaitir/node-desafio2-novo/blob/master/LICENSE)
![](https://img.shields.io/github/package-json/v/osvaldokalvaitir/node-desafio2-novo.svg)
![](https://img.shields.io/github/last-commit/osvaldokalvaitir/node-desafio2-novo.svg?color=red)
![](https://img.shields.io/github/languages/top/osvaldokalvaitir/node-desafio2-novo.svg?color=yellow)
![](https://img.shields.io/github/languages/count/osvaldokalvaitir/node-desafio2-novo.svg?color=lightgrey)
![](https://img.shields.io/github/languages/code-size/osvaldokalvaitir/node-desafio2-novo.svg)
![](https://img.shields.io/github/repo-size/osvaldokalvaitir/node-desafio2-novo.svg?color=blueviolet)
[![made-for-VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)](https://code.visualstudio.com/)
![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

## Desafio 02. Iniciando aplicação

Crie uma aplicação do zero utilizando Express.

Nessa aplicação configure as seguintes ferramentas:

- Sucrase + Nodemon;
- ESLint + Prettier + EditorConfig;
- Sequelize (Utilize PostgresSQL ou MySQL);

Durante esse desafio você dará início a um novo projeto no Bootcamp, esse projeto será desenvolvido aos poucos até o fim da sua jornada onde você terá uma aplicação completa envolvendo back-end, front-end e mobile.

Esse projeto também será utilizado para a certificação do bootcamp, então bora pro código!

### Aplicação

A aplicação que iremos dar início ao desenvolvimento a partir de agora é um app agregador de eventos para desenvolvedores chamado Meetapp (um acrônimo à Meetup + App).

Nesse primeiro desafio vamos criar algumas funcionalidades básicas que aprendemos ao longo das aulas até aqui.

### Funcionalidades

Abaixo estão descritas as funcionalidades que você deve adicionar em sua aplicação.

#### Autenticação

Permita que um usuário se autentique em sua aplicação utilizando e-mail e senha.

- A autenticação deve ser feita utilizando JWT.
- Realize a validação dos dados de entrada;

#### Cadastro e atualização de usuários

Permita que novos usuários se cadastrem em sua aplicação utilizando nome, e-mail e senha.

Para atualizar a senha, o usuário deve também enviar um campo de confirmação com a mesma senha.

- Criptografe a senha do usuário para segurança.
- Realize a validação dos dados de entrada;