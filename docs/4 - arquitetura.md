# Arquitetura do Projeto - Manga Reader Site

## 1. Visão Geral

O projeto será estruturado em três camadas principais:

- **Frontend (Cliente)** → Interface que roda no navegador (SPA)
- **Backend (Servidor)** → API RESTful responsável por processar requisições
- **Banco de Dados** → Armazena usuários, mangás, capítulos, favoritos, etc.

---

## 2. Arquitetura Geral

[ Usuário ] ⇅ HTTP [ Frontend - React ] ⇅ REST API (JSON) [ Backend - Node.js / Express ] ⇅ Sequelize ORM [ Banco de Dados - PostgreSQL ]

---

## 3. Fluxo de Requisição (Exemplo)

1. O usuário acessa o site e faz login.
2. O React envia uma requisição `POST /api/login` para o backend.
3. O backend valida os dados, gera um token JWT e retorna para o frontend.
4. O token é armazenado no navegador (ex: `localStorage`).
5. O frontend usa o token para buscar dados protegidos (ex: favoritos).
6. O backend valida o token e responde com os dados do PostgreSQL.

---

## 4. Estrutura de Pastas (Sugestão)

/frontend /public /src /components /pages /services       # APIs /styles /utils
/backend /controllers /routes /models /middlewares 
    /services /config/assets /mangas /capitulos
    /docs (...documentação)

---

## 5. Segurança

- JWT para autenticação
- Senhas criptografadas com bcrypt
- Verificação de token em rotas protegidas
- CORS habilitado corretamente

---

## 6. Escalabilidade Futura (Ideias)

- Separar API de autenticação em microsserviço
- Usar CDN para imagens (Cloudflare, Cloudinary)
- Adicionar Redis para cache
- Utilizar Docker para facilitar deploy

---

> ⚠️ Esta arquitetura pode ser adaptada conforme o projeto evoluir.
