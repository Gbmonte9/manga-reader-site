# API Externa - MangaDex

## Base URL

https://api.mangadex.org


## Exemplo de busca por título

### Endpoint

### GET /manga?title=one piece

### Resposta simplificada
```json
{
  "data": [
    {
      "id": "123abc",
      "attributes": {
        "title": { "en": "One Piece" },
        "status": "ongoing",
        "description": { "en": "Pirate adventure" }
      }
    }
  ]
}
```