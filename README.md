# meu-projeto-back-end
<h1 align="center">TypeScript + Express Backend</h1> <p align="center"> <b>Projeto de desenvolvimento de servidor com Node.js</b><br> <sub>visual moderno • organizado • interativo • colorido</sub> </p> <p align="center"> <a href="#sobre"><img src="https://img.shields.io/badge/sobre-ff69b4?style=for-the-badge"></a> <a href="#instalacao"><img src="https://img.shields.io/badge/instalação-8a2be2?style=for-the-badge"></a> <a href="#estrutura"><img src="https://img.shields.io/badge/estrutura-00cfff?style=for-the-badge"></a> <a href="#execucao"><img src="https://img.shields.io/badge/execução-00ff9c?style=for-the-badge"></a> </p>
<a name="sobre"></a> Sobre

Este projeto apresenta a criação de um servidor backend utilizando TypeScript, Node.js e Express.

O projeto utiliza:

TypeScript
Node.js
Express
TSX
npm
HTTP
Servidor local

O servidor será executado na porta 8081.

<a name="instalacao"></a> Instalação
01 — Criar o projeto
npm init -y
npm i -D typescript @types/node tsx
npx tsc --init
02 — Instalar o Express
npm install express
npm install -D @types/express
<a name="estrutura"></a> Estrutura do projeto
meu-projeto-backend/
│
├── node_modules/
│
├── src/
│   └── app.ts
│
├── package.json
│
├── package-lock.json
│
└── tsconfig.json
Servidor Express

O arquivo responsável pelo servidor será:

src/app.ts
Código do servidor
// Importa a biblioteca Express e também o tipo Express
// O Express será utilizado para criar o servidor web
import express from "express";
import type { Express } from "express";

// Cria uma aplicação Express
// A função express() devolve um objeto que representa o servidor da aplicação
const app: Express = express();

// Define a porta onde o servidor ficará disponível
// Neste caso, o servidor poderá ser acessado pela porta 8081
const PORT: number = 8081;

// Inicializa o servidor utilizando a porta definida
// O método listen() faz o servidor começar a "escutar" requisições HTTP
app.listen(PORT, () => {
  console.log(`Servidor rodando em http://localhost:${PORT}`);
});
Configuração do package.json

No arquivo package.json, configure o script:

"scripts": {
  "dev": "tsx watch src/app.ts"
}

Esse comando permite executar o arquivo TypeScript e reiniciar o servidor automaticamente quando houver alterações.

<a name="execucao"></a> Executar o projeto

No terminal, utilize:

npm run dev

Se tudo estiver funcionando corretamente, será exibido:

Servidor rodando em http://localhost:8081
Acessar o servidor

Abra o navegador e acesse:

http://localhost:8081

O servidor estará disponível localmente na porta:

8081
Progresso
Etapa	Progresso	Status
Criar projeto Node.js	██████████ 100%	Concluído
Instalar TypeScript	██████████ 100%	Concluído
Instalar Express	██████████ 100%	Concluído
Criar app.ts	██████████ 100%	Concluído
Configurar package.json	██████████ 100%	Concluído
Executar servidor	██████████ 100%	Concluído
Gráfico visual
Node.js       ▰▰▰▰▰▰▰▰▰▰ 100%
TypeScript    ▰▰▰▰▰▰▰▰▰▰ 100%
Express       ▰▰▰▰▰▰▰▰▰▰ 100%
Servidor      ▰▰▰▰▰▰▰▰▰▰ 100%
Configuração  ▰▰▰▰▰▰▰▰▰▰ 100%
Tecnologias
<p align="center"> <img src="https://img.shields.io/badge/TypeScript-ff69b4?style=for-the-badge"> <img src="https://img.shields.io/badge/Node.js-8a2be2?style=for-the-badge"> <img src="https://img.shields.io/badge/Express-00cfff?style=for-the-badge"> <img src="https://img.shields.io/badge/npm-00ff9c?style=for-the-badge"> </p>
Fluxo do projeto
npm init -y
      │
      ▼
Instalar TypeScript
      │
      ▼
Instalar Express
      │
      ▼
Criar src/app.ts
      │
      ▼
Configurar package.json
      │
      ▼
npm run dev
      │
      ▼
Servidor Express
      │
      ▼
localhost:8081
Comandos utilizados
Criar projeto
npm init -y
Instalar TypeScript
npm i -D typescript @types/node tsx
Criar configuração do TypeScript
npx tsc --init
Instalar Express
npm install express
Instalar tipos do Express
npm install -D @types/express
Executar servidor
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
├── package-lock.json
└── tsconfig.json
Autora
<p align="center"> <b>Anna Beatriz Rufino de Araújo</b> </p> <p align="center"> Desenvolvimento de Sistemas </p>
<p align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=ff69b4&height=100&section=footer"/> </p>
