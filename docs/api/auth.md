# API - Autenticação

## POST /api/login

### Descrição
Autentica o usuário e retorna um token JWT.

### Corpo da requisição (JSON)
```json
{
  "email": "usuario@email.com",
  "senha": "123456"
}
```

### Resposta (200 OK)
```json
{
  "token": "eyJhbGciOiJIUzI1NiIs...",
  "usuario": {
    "id": 1,
    "nome": "Gabriel",
    "email": "usuario@email.com"
  }
}
```

---

## POST /api/login

### Descrição
Cria uma nova conta de usuário.

### Corpo da requisição (JSON)
```json
{
  "nome": "Gabriel",
  "email": "usuario@email.com",
  "senha": "123456"
}
```

### Resposta (201 Created)

```json
{
  "mensagem": "Usuário registrado com sucesso."
}
```
---

## POST /api/logout (opcional)

### Descrição
Invalida o token no frontend (backend não precisa fazer nada).








