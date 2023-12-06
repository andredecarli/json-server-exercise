# json-server-exercise

Nesse exercicio, iremos configurar um JSON Server, que simula um backend.
O JSON Server vai ser útil para podermos testar nosso frontend e a comunicação com APIs em geral.

Para instalar o JSON Server, após criar seu repositório, inicie um projeto Node:
```
npm init -y
```
Depois disso, instale a dependência do JSON Server:
```
npm i json-server
```
Caso opte por clonar este repositório ao invés de criar o seu do zero, basta executar o seguinte comando:
```
npm install
```

Feito isto, vamos configurar nosso JSON Server:
* Crie um arquivo `db.json` na raíz de seu projeto.
* Insira um conteúdo JSON. Por exemplo:
```json
{
  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 }
  ],
  "profile": { "name": "typicode" }
}
```
* Inicie o JSON Server
```
npx json-server db.json
```
Feito isto, a rota `http://localhost:3000` estará disponível para adquirir as informações da API. Neste exemplo, as rotas são:
```
http://localhost:3000/posts
http://localhost:3000/comments
http://localhost:3000/profile
```

Para mais informações, você pode [consultar o README do JSON Server](https://github.com/typicode/json-server/tree/main)