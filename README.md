
<h1 align="center">
  Tech Challenge CEFIS 🚀
</h1>

<p align="center">
	<a href="#rocket-requisitos">O desafio</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-requisitos">Requisitos</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#rocket-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#information_source-como-usar">Como usar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#scroll-scripts-disponíveis">Scripts disponíveis</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
	<a href="#earth_americas-rotas-da-api">Rotas da API</a>
</p>

## :rocket: O desafio
O projeto "Desafio Kanban - Frontend" tem como objetivo desenvolver a interface de um quadro Kanban, seguindo o layout fornecido pela empresa [CEFIS](https://cefis.com.br/) e utilizando dados fictícios. Os requisitos obrigatórios incluem a implementação das colunas "A Fazer", "Fazendo" e "Feito", permitindo que os cards sejam arrastáveis entre essas colunas. Além disso, as tecnologias requisitadas são Next.js e Tailwind CSS. 

Entre as melhorias implementadas, destaco a criação de colunas personalizadas e arrastáveis, conforme demonstrado nos GIFs abaixo. Apenas as colunas personalizadas podem ser apagadas, enquanto as colunas padrão ("A Fazer", "Fazendo" e "Feito") permanecem fixas. O usuário também pode filtrar as tarefas pelo nome do projeto, solicitante, executante ou inserindo o nome ou ID da tarefa. Todas as colunas têm títulos editáveis ao clicar neles, e os solicitantes de cada tarefa são gerados aleatoriamente. Vale mencionar que, no código, os dados são buscados tanto das rotas da API disponibilizadas abaixo quanto de forma local para exibição na Vercel, então alguns trechos de código ficaram maiores pela inserção dos dados fictícios. Para finalizar, o projeto também é responsivo para celulares, tablets e outros computadores. O produto final pode ser acessado através deste [link](https://tech-challenge-cefis.vercel.app/)

![Demonstração do produto final](docs/KanbanBoardDemoPart1.gif)
![Demonstração do produto final](docs/KanbanBoardDemoPart2.gif)

## :memo: Requisitos

| Ferramenta| Versão  | Descrição                                    |
|-----------|---------|----------------------------------------------|
| [NodeJS](https://nodejs.org/en/)              | 20.13.1 | Ambiente de execução Javascript server-side  |
| [NPM](https://www.npmjs.com/)                 | 10.8.1 | Gerenciador de pacotes JS                    |
| [Git](https://git-scm.com/)           | | |


## :man_technologist: Tecnologias

Este projeto está sendo desenvolvido com as seguintes tecnologias:

-  Linguagem: [Typescript](https://www.typescriptlang.org/);
-  Biblioteca JS para front-end: [ReactJS](https://reactjs.org/);
-  Estilização: [Tailwind](https://tailwindcss.com/) + [React-Icons](https://react-icons.github.io/react-icons/) + [Chakra UI](https://v2.chakra-ui.com/);
-  Framework Fullstack: [Next.js](https://nextjs.org/);
-  Gerenciamento de estados: [Zustand](https://zustand-demo.pmnd.rs/);
-  Padronização: [Rocketseat ESLint Config](https://github.com/Rocketseat/eslint-config-rocketseat) + [ESLint](https://eslint.org/) + [Prettier](https://prettier.io/);
-  Git Hook: [Husky](https://typicode.github.io/husky/#/);

## :information_source: Como usar

Um tutorial em vídeo está disponível neste [link](https://youtu.be/sV-zAxocerc).

```bash
# Clonar este repositório
$ git clone https://github.com/arthurbfonseca27/tech-challenge-cefis.git
# Ir para o repositório
$ cd tech-challenge-cefis
# Instalar as dependências
$ npm install
# Rodar a aplicação em ambiente de desenvolvimento
$ npm run dev
```
## :scroll: Scripts disponíveis

- `dev`: Inicia a aplicação;
- `build`: Build da aplicação;
- `prepare`:  Inicializa o Husky;
- `lint`: Escaneia a aplicação verificando e consertando erros nas aplicação;


## :earth_americas: Rotas da API
- GET `/tasks`: API para listar tarefas;
- GET `/requesters`: API para listar solicitantes;
- GET `/executers`: API para listar executantes;
