# teste-webhook

Repositório de teste para recebimento de webhooks.

## Objetivo

Armazenar exemplos e código mínimo para validar webhooks (GitHub, Discord, etc.) localmente.

## Como usar

- Configure seu servidor que receberá o webhook (por exemplo, em Node/Express ou Nest).
- Defina a variável de ambiente `GITHUB_WEBHOOK_SECRET` com o secret usado nos testes.

Exemplo rápido com `curl` (substitua a URL pela do seu servidor):

```bash
curl -X POST -H "Content-Type: application/json" \
  -d '{"action":"test"}' \
  http://localhost:3000/api/webhooks/github
```

## Próximos passos

- Adicionar um exemplo de servidor que verifica `X-Hub-Signature-256`.
- Incluir scripts de teste automatizados.

--
Criado automaticamente no workspace.
