# Middlewares

- `authMiddleware.js` → Verifica se o token JWT é válido
- `errorHandler.js` → Captura e retorna erros com status adequado
- `validateBody.js` → Valida o corpo da requisição (login, registro, etc.)

Uso no Express:

```js
app.use('/api/favoritos', authMiddleware, favoritosRoutes);
```

---
# Autenticação JWT

- Ao logar, o backend gera um token com `jsonwebtoken`
- Esse token é enviado no header `Authorization: Bearer <token>`
- O middleware verifica o token em rotas protegidas

Senha criptografada com `bcrypt`:

```js
const hash = await bcrypt.hash(senha, 10);
```

---