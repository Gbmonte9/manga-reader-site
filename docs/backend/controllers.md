# Controllers

- `authController.js` → Lógica de login e registro
- `mangaController.js` → Listagem e busca de mangás
- `capituloController.js` → Capítulos e leitura
- `usuarioController.js` → Perfil, favoritos, progresso

Cada controller importa seu service e envia resposta via `res.status().json()`