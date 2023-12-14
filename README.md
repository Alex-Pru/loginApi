<h1>Olá! Bem-Vindo à LoginAPI</h1>

<h2>Descrição: 🗣️</h2>

<p>Esta é uma API de login simples que possui criptografia Hash na senha, JWT como Token, Persistência de Dados e outras características.</p>

<h2>Auxílio para testes: 👨‍💻👩‍💻</h2>

<p>Podem ser utilizadas ferramentas específicas para testes de API ou comandos no prompt para testar as rotas, requisições, erros e respostas. Demonstrarei como testar as mesmas a partir do git Bash: </p><br>

<p>Utilizando o comando: "curl -X POST -H "Content-Type: application/json" -d '{
  "nome": "seu_Nome",
  "email": "seu_Email@gmail.com",
  "senha": "sua_Senha",
  "telefones": [
    {"numero": "123456789", "ddd": "11"}
  ]
}'  https://login-escribo-api.onrender.com/register" é possível testar a rota de registro, esta rota retorna dados referentes a criação do usuário no MongoDB.</p>

<br>
<br>

<p>Utilizando o comando: "curl -X POST -H "Content-Type: application/json" -d '{
  "email": "seu_Email@gmail.com",
  "senha": "sua_Senha"
}' https://login-escribo-api.onrender.com/login" é possível testar a rota de login, esta rota retorna os mesmos dados de criação da conta, agora com adição do campo "ultimo_login" que atualiza toda vez que o usuário faz login e um novo token que será usado futuramente.</p>

<br>
<br>

<p>Utilizando o comando: "curl -H "Authorization: Bearer seuToken " https://login-escribo-api.onrender.com/api/protegida" é possível testar a rota que retorna o usuário, a mesma diz se a rota está segura ou não, além de responder com algumas informações do usuário.</p>
