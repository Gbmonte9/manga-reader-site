# Rotas do Backend

## Prefixo principal: `/api`

### Autenticação
- `POST /api/login` → Login do usuário
- `POST /api/register` → Criação de conta

### Mangás
- `GET /api/mangas` → Listar mangás
- `GET /api/mangas/:id` → Detalhes de um mangá
- `GET /api/mangas/:id/capitulos` → Capítulos do mangá

### Capítulos
- `GET /api/capitulos/:id` → Detalhes do capítulo + imagens

### Usuário
- `GET /api/usuario` → Dados do perfil (protegido)
- `GET /api/favoritos` → Lista de favoritos
- `POST /api/favoritos` → Adicionar favorito
- `DELETE /api/favoritos/:id` → Remover favorito