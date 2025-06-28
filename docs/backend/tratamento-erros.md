# Tratamento de Erros

- Criar middleware `errorHandler.js`
- Padronizar erros com código, mensagem e contexto

Exemplo:

```json
{
  "erro": "Usuário não encontrado",
  "status": 404
}
```

No código:

```js
app.use((err, req, res, next) => {
  res.status(err.status || 500).json({
    erro: err.message || 'Erro interno no servidor'
  });
});
```


---