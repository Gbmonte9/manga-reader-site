# Estratégia de Integração com API Externa

## Cenário

Queremos buscar mangás e capítulos automaticamente de uma fonte pública como MangaDex, reduzindo a necessidade de subir imagens manualmente.

## Possibilidades:

- Backend acessa a API externa e armazena os dados localmente
- Frontend consome direto da API externa (menos seguro, mas mais leve)
- Cachear os dados da API em banco local (ex: cron job 1x por dia)

## Decisão (temporária):
Vamos começar consumindo direto da API externa no backend e salvar os resultados relevantes no banco local.