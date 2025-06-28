# Integração com a API

- Bibliotecas: Axios
- Token JWT incluído no header:

```js
axios.get('/api/favoritos', {
  headers: {
    Authorization: `Bearer ${token}`
  }
})
```

Todas as chamadas à API são centralizadas em src/services/api.js