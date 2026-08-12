# meu-projeto-back-end
# TypeScript + Express Backend

> Projeto de desenvolvimento de servidor com Node.js, TypeScript e Express.

**Backend** • **TypeScript** • **Node.js** • **Express**

---

# Sobre o projeto

Este projeto apresenta a criação de um servidor backend utilizando:

- TypeScript
- Node.js
- Express
- TSX
- npm
- HTTP

O servidor será executado na porta **8081**.

---

# Objetivos

- Criar um servidor HTTP
- Utilizar TypeScript
- Configurar o Express
- Utilizar o TSX
- Executar o servidor localmente
- Trabalhar com uma estrutura básica de backend

---

# 1. Preparando o ambiente

Primeiramente, criamos o projeto Node.js e instalamos as ferramentas necessárias.

## Criar o projeto

```bash
npm init -y
npm i -D typescript @types/node tsx
npx tsc --init
2. Instalando o Express

Instale o framework Express e os tipos necessários para TypeScript.

npm install express
npm install -D @types/express
3. Criando a estrutura do projeto

Crie a pasta src e, dentro dela, o arquivo app.ts.

A estrutura ficará:

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
4. Criando o servidor

O arquivo responsável pelo servidor será:

src/app.ts
Código
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
5. Entendendo o código
Importação do Express

Primeiro importamos a biblioteca Express e o tipo Express.

import express from "express";
import type { Express } from "express";
Criação da aplicação

A função express() cria a aplicação do servidor.

const app: Express = express();
Definição da porta

A porta utilizada pelo servidor será a 8081.

const PORT: number = 8081;
Inicialização do servidor

O método listen() inicia o servidor.

app.listen(PORT, () => {
  console.log(`Servidor rodando em http://localhost:${PORT}`);
});

Quando o servidor iniciar corretamente, será exibida a mensagem:

Servidor rodando em http://localhost:8081
6. Configurando o package.json

Abra o arquivo:

package.json

Localize a propriedade "scripts" e configure:

"scripts": {
  "dev": "tsx watch src/app.ts"
}

O comando:

npm run dev

executará:

tsx watch src/app.ts

O watch permite que o servidor seja atualizado automaticamente quando o arquivo app.ts for alterado.

7. Executando o servidor

Depois de realizar todas as configurações, execute:

npm run dev

O resultado esperado será:

Servidor rodando em http://localhost:8081
8. Acessando o servidor

Abra o navegador e acesse:

http://localhost:8081

O servidor estará disponível localmente na porta:

8081

9. Progresso
Etapa	Progresso	Status
Criar projeto Node.js	██████████ 100%	Concluído
Instalar TypeScript	██████████ 100%	Concluído
Instalar Express	██████████ 100%	Concluído
Criar app.ts	██████████ 100%	Concluído
Configurar package.json	██████████ 100%	Concluído
Executar servidor	██████████ 100%	Concluído
10. Gráfico visual
Node.js
████████████████████ 100%

TypeScript
████████████████████ 100%

Express
████████████████████ 100%

Servidor
████████████████████ 100%

Configuração
████████████████████ 100%
11. Tecnologias utilizadas
Tecnologia	Utilização
TypeScript	Linguagem utilizada no projeto
Node.js	Ambiente de execução
Express	Framework para criação do servidor
TSX	Execução de TypeScript
npm	Gerenciamento de pacotes
12. Fluxo do projeto
Criar projeto
      ↓
Instalar TypeScript
      ↓
Configurar TypeScript
      ↓
Instalar Express
      ↓
Criar src/app.ts
      ↓
Configurar package.json
      ↓
Executar npm run dev
      ↓
Servidor Express
      ↓
localhost:8081
13. Comandos utilizados
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
Executar o servidor
npm run dev
14. Estrutura final
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
15. Resultado

Depois de executar:

npm run dev

o servidor ficará disponível em:

http://localhost:8081

Mensagem esperada:

Servidor rodando em http://localhost:8081
Autora

Anna Beatriz Rufino de Araújo

Curso: Desenvolvimento de Sistemas

Projeto concluído
████████████████████████████████████████ 100%

TypeScript + Express Backend
