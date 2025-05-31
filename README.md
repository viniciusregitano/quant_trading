# QuantTrading Repository

Structure generated automatically.

## Local Dev Stack (T-0.1)

### Pré‑requisitos
* Docker ≥ 24
* Docker Compose v2
* 4 GB RAM livres e ~2 GB espaço em disco (ClickHouse)

### Subindo o ambiente
```bash
# 1. clone
$ git clone main quant_trading && cd quant_trading

# 2. crie o arquivo de variáveis de ambiente
$ cp .env.example .env  # edite MODEL_URI se necessário

# 3. construa imagens locais (ou puxe as do CI)
$ docker compose -f docker/docker-compose.yml pull  # ou build

# 4. inicie os serviços
$ docker compose -f docker/docker-compose.yml up -d

# 5. verifique status/health
$ docker compose ps