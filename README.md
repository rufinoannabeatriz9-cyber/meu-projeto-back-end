# Backend com Node.js, TypeScript e Express

> Projeto desenvolvido para aprender a configurar um ambiente **Backend** utilizando **Node.js**, **TypeScript** e **Express**.

---

## Tecnologias

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![NPM](https://img.shields.io/badge/NPM-CB3837?style=for-the-badge&logo=npm&logoColor=white)

---

## Sumário

- [Sobre o projeto](#sobre-o-projeto)
- [Preparando o ambiente](#preparando-o-ambiente)
- [Instalando o Express](#instalando-o-express)
- [Estrutura do projeto](#estrutura-do-projeto)
- [Criando o servidor](#criando-o-servidor)
- [Configurando o package.json](#configurando-o-packagejson)
- [Executando o servidor](#executando-o-servidor)
- [Como funciona](#como-funciona)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Comandos principais](#comandos-principais)
- [Status](#status)

---

## Sobre o projeto

Este projeto apresenta a configuração inicial de um ambiente **Backend** utilizando **TypeScript** e **Express**.

O objetivo é criar um servidor HTTP simples que ficará disponível na porta `8081`.

### Fluxo do projeto

text
Cliente
   |
   | Requisição HTTP
   v
Express
   |
   | Processamento
   v
Servidor
   |
   v
localhost:8081
Preparando o ambiente

Primeiro, inicialize o projeto Node.js:

npm init -y

Depois, instale o TypeScript e as ferramentas necessárias:

npm i -D typescript @types/node tsx

Crie o arquivo de configuração do TypeScript:

npx tsc --init
Função de cada comando
Comando	Função
npm init -y	Cria o arquivo package.json
npm i -D typescript	Instala o TypeScript
@types/node	Adiciona os tipos do Node.js
tsx	Executa arquivos TypeScript
npx tsc --init	Cria o tsconfig.json
Instalando o Express

Instale o framework Express:

npm install express

Depois, instale os tipos do Express para o TypeScript:

npm install -D @types/express

O Express facilita a criação de servidores web e APIs utilizando Node.js.

Estrutura do projeto

A estrutura inicial ficará assim:

meu-projeto-backend/
│
├── node_modules/
│
├── src/
│   └── app.ts
│
├── package.json
│
└── tsconfig.json
Criando o servidor

Crie o arquivo:

src/app.ts

Dentro dele, adicione:

import express from "express";
import type { Express } from "express";

const app: Express = express();

const PORT: number = 8081;

app.listen(PORT, () => {
    console.log(`Servidor rodando em http://localhost:${PORT}`);
});
Como funciona
Importando o Express
import express from "express";
import type { Express } from "express";

Importa a biblioteca Express e o tipo Express para utilização com TypeScript.

Criando a aplicação
const app: Express = express();

Cria uma aplicação Express que será utilizada como nosso servidor.

Definindo a porta
const PORT: number = 8081;

Define a porta 8081 onde o servidor ficará disponível.

Iniciando o servidor
app.listen(PORT, () => {
    console.log(`Servidor rodando em http://localhost:${PORT}`);
});

O método listen() inicia o servidor e faz com que ele fique aguardando requisições HTTP.

Configurando o package.json

Abra o arquivo package.json.

Na propriedade "scripts", adicione:

"scripts": {
    "dev": "tsx watch src/app.ts"
}

Esse comando permite executar o servidor utilizando o tsx.

O watch também permite que o servidor seja reiniciado automaticamente quando o código for alterado.

Executando o servidor

No terminal, execute:

npm run dev

Se tudo estiver funcionando corretamente, será exibido:

Servidor rodando em http://localhost:8081

O servidor estará disponível em:

http://localhost:8081

Fluxo de execução
npm run dev
      |
      v
tsx watch src/app.ts
      |
      v
Express
      |
      v
Servidor HTTP
      |
      v
Porta 8081
      |
      v
http://localhost:8081
Tecnologias utilizadas
Tecnologia	Função
Node.js	Ambiente para execução do Backend
TypeScript	Linguagem utilizada no desenvolvimento
Express	Framework para criação do servidor
tsx	Execução de arquivos TypeScript
npm	Gerenciamento de pacotes
Comandos principais
Inicialização
npm init -y
Instalação do TypeScript
npm i -D typescript @types/node tsx
Configuração do TypeScript
npx tsc --init
Instalação do Express
npm install express
Tipos do Express
npm install -D @types/express
Executar o servidor
npm run dev
Estrutura final
meu-projeto-backend/
│
├── node_modules/
│
├── src/
│   └── app.ts
│
├── package.json
│
└── tsconfig.json
Status

Projeto desenvolvido para estudos de Backend, Node.js, TypeScript e Express.
