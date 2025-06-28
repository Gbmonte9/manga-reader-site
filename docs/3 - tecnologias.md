# Tecnologias do Projeto - Manga Reader Site

## 1. Frontend

- **HTML5, CSS3 e JavaScript** – Estrutura, estilo e interatividade básica.
- **Framework:** React.js *(SPA e componentes reutilizáveis)*
- **Estilização:** Bootstrap (com tema escuro) + Tailwind CSS para detalhes visuais.
- **Gerenciamento de Estado:** Context API (pode ser trocado por Redux se necessário)
- **Roteamento:** React Router DOM
- **Consumo de API:** Axios ou Fetch API

## 2. Backend

- **Plataforma:** Node.js com Express.js
- **Banco de Dados:** PostgreSQL
- **ORM:** Sequelize ou Prisma
- **Autenticação:** JWT (JSON Web Token)
- **Hash de senha:** bcrypt
- **Serviços RESTful:** CRUD de usuários, mangás, capítulos, favoritos, etc.

## 3. Armazenamento de Imagens

- **Local** (durante desenvolvimento)
- **Produção:** considerar S3 (Amazon), Cloudinary ou outros

## 4. DevOps e Ferramentas

- **Gerenciador de pacotes:** npm ou yarn
- **Versionamento:** Git + GitHub
- **Ambiente local:** Docker (opcional, mas útil)
- **Hospedagem Frontend:** Vercel ou Netlify
- **Hospedagem Backend:** Render, Railway, ou VPS (caso opte por algo mais robusto)
- **Banco em produção:** Supabase ou ElephantSQL (PostgreSQL gratuito)

## 5. Extras/Opcionais

- **pdfkit ou jsPDF** – Geração de PDF para capítulos
- **Socket.io** – Para comentários em tempo real (se usar chat)
- **Lodash ou Day.js** – Utilidades para manipulação de dados e datas
- **Cloudflare** – CDN e segurança de imagens

---

> ⚠️ As tecnologias podem ser alteradas ou reduzidas conforme o escopo. Comece simples e vá evoluindo conforme a necessidade.
