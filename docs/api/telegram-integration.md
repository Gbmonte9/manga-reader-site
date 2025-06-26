# 🤖 Integração com Telegram para Obtenção de Mangás

## Objetivo
Utilizar canais do Telegram como fonte para obter capítulos de mangás, automatizando a coleta e o armazenamento.

## Funcionamento (ideia inicial)
1. Bot ou script acessa canal X
2. Pega as mensagens com imagens
3. Baixa as imagens por ordem
4. Armazena em `/public/mangas/{titulo}/{capitulo}/`
5. Atualiza o banco com novo capítulo

## Possíveis Tecnologias
- `python-telegram-bot`
- `telethon`
- `node-telegram-bot-api`

## Riscos
- Problemas legais se os mangás forem protegidos por copyright
- Canais que mudam links ou bloqueiam automação
- APIs do Telegram com limite de taxa (rate limit)

## Status
🔁 Em estudo (ideia em análise)