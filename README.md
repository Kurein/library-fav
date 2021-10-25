# json-server-base-library-fav

Esse é o repositório com uma base de uma API de Biblioteca, onde existem variados livros que podem ser colocados em uma lista de favoritos de cada usuário

## Endpoints

A API conta com um total de 6 Endpoits sendo eles relacionados com: criação de usuário, registrar, logar, ver a biblioteca, adicionar livro na lista de favoritos, ver a lista de favoritos

<h2 align ='center'> Cadastro e Login </h2>

### Cadastro

Um Endpoint básico de cadastro de usuário

POST /register <br/>

body:

{ <br/>
"email":<br/>
"password":<br/>
"name":<br/>
"age":<br/>
}<br/>

### Login

Um outro Endpoint básico para logar o usuário

POST /login <br/>

body:

{<br/>
"email":<br/>
"password":<br/>
}<br/>

<h2 align ='center'> Endpoints que não precisam de uma autenticação </h2>

### Lista de Usuários

GET /users <br/>

E para ter acesso a um usuário em específico

GET /users/id <br/>

### Biblioteca

GET /books <br/>

<h2 align ='center'> Endpoints que precisam de uma autenticação </h2>

### Adicionar item aos favoritos

POST /favorites <br/>

body:

{<br/>
"name":<br/>
"pages":<br/>
"author":<br/>
"userId":<br/>
}<br/>

### Lista de favoritos

GET /favorites <br/>

Para ter acesso a um favorito em específico

GET /favorites/id <br/>
