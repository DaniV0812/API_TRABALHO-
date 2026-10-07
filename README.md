# Loja Neo

Estrutura esperada:

```
index.js  db.js  migration.js  validacao.js  package.json  .env  .gitignore
front/  index.html  script.js  style.css  produtos.json
```

1. `npm install`
2. Crie o `.env` (o arquivo enviado se chamava `_env`) com DB_HOST, DB_PORT, DB_USER, DB_PASSWORD, DB_NAME e JWT_SECRET
3. `node migration.js`   (cria a tabela Clientes ou adiciona as colunas novas: cep, rua, numero, bairro, cidade, estado, data_nascimento)
4. `node index.js`
5. Abra http://localhost:3002

Rotas: POST /Clientes, POST /login, GET /Clientes/perfil (token), GET /produtos, GET /produtos/:id

No cadastro, ao digitar o CEP completo o endereço é preenchido via ViaCEP.
