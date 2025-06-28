# API - Mangás

## GET /api/mangas

### Descrição
Lista todos os mangás disponíveis, com paginação.

### Query Params
- `?pagina=1`
- `?busca=naruto`

### Resposta
```json
[
  {
    "id": 5,
    "titulo": "One Piece",
    "capa": "/assets/mangas/onepiece.jpg",
    "status": "Em lançamento"
  }
]
```

---

## GET /api/mangas

### Descrição
Detalhes de um mangá específico, incluindo capítulos.

### Resposta
```json
{
  "id": 5,
  "titulo": "One Piece",
  "autor": "Eiichiro Oda",
  "descricao": "Piratas, aventura e tesouros.",
  "capitulos": [
    { "id": 101, "numero": 1, "titulo": "Romance Dawn" },
    { "id": 102, "numero": 2, "titulo": "O garoto de palha" }
  ]
}
```

---

### 📌 Dica
Na `estrutura-geral.md`, você pode anotar coisas como:
- Formato padrão de erro
- Necessidade de token em rotas protegidas
- Status HTTP retornados

---

Se quiser, posso montar agora o `capitulos.md` ou `usuarios.md`. Só me dizer qual endpoint você quer documentar primeiro!

