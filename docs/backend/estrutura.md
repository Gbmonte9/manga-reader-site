# Estrutura do Backend

## Tecnologias principais
- Node.js com Express
- PostgreSQL com Sequelize
- Autenticação JWT
- Senhas criptografadas com bcrypt

## Estrutura de Pastas

/backend
/controllers → Funções que recebem e tratam as requisições
/routes → Arquivos com os endpoints (ex: auth.js, manga.js)
/models → Definições das tabelas com Sequelize
/middlewares → Validações, autenticação, tratamento de erro
/services → Regras de negócio (ex: lógica de favoritos)
/config → Conexão com banco, variáveis de ambiente
app.js → Configuração geral do Express
server.js → Inicializa o servidor

Copy
Edit
