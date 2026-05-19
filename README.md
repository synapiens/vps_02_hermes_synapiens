# VPS Hermes Nexus

## Painel 
https://painel.integrator.host/dashboard
User: pmazzia@gmail.com

## VPS
- IP : 209.50.254.173
- PWD : 8bxG4OJR8Tk52peN
- S.O. : Ubuntu 24.04 LTS (x86_64)


## Instalações

### Portainer ( Orion Setup )

- Link do Portainer: porto.hermes.synapiens.com.br
- Usuario do Portainer: mazzia
- Senha do Portainer: To7@pc2102Tech
- Nome do Servidor: HermesNexus
- Rede interna: HermesNet
- Email: hermes@synapiens.com.br

### N8N ( Orion Setup )

- Dominio do N8N: n8n.hermes.synapiens.com.br
- Dominio para o Webhook: webhook.hermes.synapiens.com.br
- Email do SMTP: hermes@synapiens.com.br
- Usuário do SMTP: hermes@synapiens.com.br
- Senha do Email: To7@pc2102
- Host SMTP do Email: mail.synapiens.com.br
- Porta SMTP do Email: 465
- Secure SMTP do Email: true

### Evolution GO

- Link Evolution GO: https://evogo.hermes.synapiens.com.br/manager
- Global: evo-8bxG4OJR8Tk52peN-hermes-2026

### Ollama

Domínio : ollama.hermes.synapiens.com.br
- Rede    : HermesNet
- Modelos  :
     - qwen2.5:1.5b  (~1.0 GiB — cabe nos 3.3 GiB disponíveis)
     - qwen2.5:3b  (~1.0 GiB — cabe nos 3.3 GiB disponíveis)
- CPU-only: sem GPU nessa VPS

### Chatwoot

- Dominio do Chatwoot: chatwoot.hermes.synapiens.com.br
- Nome da Empresa: HermesNexus
- Email do SMTP: hermes@synapiens.com.br
- User do SMTP: hermes@synapiens.com.br
- Senha do SMTP: To7@pc2102
- Host SMTP: mail.synapiens.com.br
- Porta SMTP: 465
- User : hermes@synapiens.com.br
- Pws: To7@pc2102


## INFRA

### Supabase

- Conta : Git Synapiens
- Organizacao : Synapiens Site e Produto
- Projeto : hermes_nexus
- URL : https://yawmxrcpqwpnfmpvlamq.supabase.co
- Chave Publicacao : sb_publishable_rowNwnw8MpPmejl5ZXbQsA_cXxARtO_
- String JDBC : postgresql://postgres:[YOUR-PASSWORD]@db.yawmxrcpqwpnfmpvlamq.supabase.co:5432/postgres
- Host: aws-1-us-east-1.pooler.supabase.com
- port: 6543
- database: postgres
- user: postgres.yawmxrcpqwpnfmpvlamq

### QDrant
- URL : cloud.qdrant.io
- Google : synapiens@gmail.com
- API Key : eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhY2Nlc3MiOiJtIiwic3ViamVjdCI6ImFwaS1rZXk6MjAxNWY3MDAtZjdjZi00YmZkLTg5NWEtNmM4ZGFiOTNlOGE0In0.VFWn8oKTC7IEgTOHSLiMn5eg1P8juHU00rxzzjy_Syg
- Cluster EndPoint : https://5eb4638e-a44d-4f18-95e3-fb376c8cabd7.eu-west-2-0.aws.cloud.qdrant.io
- Python
```
from qdrant_client import QdrantClient

qdrant_client = QdrantClient(
    url="https://5eb4638e-a44d-4f18-95e3-fb376c8cabd7.eu-west-2-0.aws.cloud.qdrant.io:6333", 
    api_key="eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhY2Nlc3MiOiJtIiwic3ViamVjdCI6ImFwaS1rZXk6MjAxNWY3MDAtZjdjZi00YmZkLTg5NWEtNmM4ZGFiOTNlOGE0In0.VFWn8oKTC7IEgTOHSLiMn5eg1P8juHU00rxzzjy_Syg",
)

print(qdrant_client.get_collections())
```
- JS
```
import {QdrantClient} from '@qdrant/js-client-rest';

const client = new QdrantClient({
    url: 'https://5eb4638e-a44d-4f18-95e3-fb376c8cabd7.eu-west-2-0.aws.cloud.qdrant.io:6333',
    apiKey: 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhY2Nlc3MiOiJtIiwic3ViamVjdCI6ImFwaS1rZXk6MjAxNWY3MDAtZjdjZi00YmZkLTg5NWEtNmM4ZGFiOTNlOGE0In0.VFWn8oKTC7IEgTOHSLiMn5eg1P8juHU00rxzzjy_Syg',
});

try {
    const result = await client.getCollections();
    console.log('List of collections:', result.collections);
} catch (err) {
    console.error('Could not get collections:', err);
}
```

## Vaults

### DeepSeek
```
{
  "deepseek": {
    "type": "api",
    "key": "sk-5464b55499814c87ae3093be484f2cca"
  }
}
```
