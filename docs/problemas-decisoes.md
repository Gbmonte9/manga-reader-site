# Problemas e Decisões - Manga Reader Site

## 1. Armazenamento de Imagens

**Problema:** Onde e como armazenar as páginas dos capítulos?  
**Opções consideradas:**
- Armazenar localmente (durante o desenvolvimento)
- Usar um serviço como Cloudinary
- Criar servidor próprio de arquivos com Express

**Decisão:** Usar armazenamento local durante o desenvolvimento para simplicidade, com possibilidade de migrar para Cloudinary na produção.

---

## 2. Autenticação do Usuário

**Problema:** Como autenticar e proteger as rotas do backend?  
**Opções:**
- Sessions com cookies
- JWT (JSON Web Token)

**Decisão:** Usar JWT por ser mais leve e compatível com SPA (React).  
**Complemento:** Armazenar o token no `localStorage`, com middleware no backend para validar em cada requisição protegida.

---

## 3. Organização do Frontend

**Problema:** Como separar componentes e páginas no React?  
**Opções:**
- Tudo junto em `/components`
- Separar por função (pages, components, services)

**Decisão:** Separar em `/components` (reutilizáveis), `/pages` (rotas principais), `/services` (requisições à API), `/utils` (funções auxiliares).  
**Justificativa:** Manutenção e organização mais clara.

---

## 4. Banco de Dados: Escolha do ORM

**Problema:** Qual ORM usar para conectar com PostgreSQL?  
**Opções:**
- Sequelize
- Prisma
- Knex

**Decisão:** Sequelize por familiaridade e documentação sólida.  
**Observação:** Prisma será considerado futuramente por sua tipagem forte e migrações mais visuais.

---

## 5. Hospedagem

**Problema:** Onde hospedar backend e frontend?  
**Decisão parcial:**
- Frontend: Vercel
- Backend: Render (gratuito com suporte a Node)
- Banco de dados: ElephantSQL (para dev), Supabase (para produção)

---

## 6. Imagens com nomes longos

**Problema:** Algumas imagens têm nomes com espaços ou acentos que quebram no navegador.  
**Decisão:** Padronizar os nomes de arquivos (sem espaços, acentos ou caracteres especiais) e salvar no banco apenas o caminho relativo.