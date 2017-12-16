# Criando Aplicativo de tarefas com Ionic 3, typescript e Firebase 
## Descrição
<p style="text-align: justify;">A aplicação mobile desenvolvida é um simples gerenciador de tarefas criado com ionic 3 e integrado aos serviços do Firebase. Ela fornece exemplos dos serviços de autenticação e de banco de dados real time do Firebase.</p>

## Como testar o AnotApp
Clone o projeto usando o git:

```bash
$ git clone https://github.com/nunesdaniel/AnotApp.git
```

Para instalar o **Ionic framework** verifique que tenha o *Node.js* e o *NPM* instalados na sua máquina e, em seguida, digite no terminal:

```bash
$ npm install -g ionic cordova
```

Se já tiver o *Ionic* instalado e quiser atualizar, digite no terminal:

```bash
$ npm update -g ionic
```

Para verificar a versão do *Ionic* instalada:
```bash
$ ionic -v
```

Navegue até a pasta do projeto pelo terminal e instale as dependências com o seguinte comando:

```bash
$ npm install
```

Para adicionar os serviços do Firebase no projeto, foi usado a biblioteca *AngularFire2*. Para incluir a biblioteca digite:

```bash
$ npm install firebase angularfire2
```

Crie o arquivo config.ts com as configurações do Firebase na raiz da pasta src:

```bash
export const config = {
  apiKey: "",
  authDomain: "",
  databaseURL: "",
  projectId: "",
  storageBucket: "",
  messagingSenderId: ""
};
```

Execute o projeto:

```bash
$ ionic serve --lab
```

Caso apresente erro devido a versão diferente do node, digite:

```bash
$ npm rebuild node-sass --force
```

Novamente rode o projeto:

```bash
$ ionic serve --lab
```

**Creditos:** Gustavo Pinho

**Links Externos:**
 - [NodeJS](https://nodejs.org/en/)
 - [Ionic](https://ionicframework.com/)
 - [Angular](https://angular.io/)
 - [Typescript](https://www.typescriptlang.org/)
