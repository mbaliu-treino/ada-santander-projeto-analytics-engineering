# README - TECH

## Arquitetura do Ambiente

* Postgres e PgAdmin monstados em Dockers

### Requerimentos

* docker >= 24.0.6+
* docker-compose
* Python >=

### TL:RD

1. Clonar e baixar o repositório
2. Na linha de comando mudar para a pasta raiz do projeto `cd proj-airbnb`
3. Executar o comando do Docker `docker compose up -d`

### Variáveis de Ambiente

Este arquivo Docker-Compose possui as seguintes variáveis de ambiente:

* `POSTGRES_USER`: o valor padrão é `postgres`
* `POSTGRES_PASSWORD`: o valor padrão é `secret`
* `POSTGRES_DB`: o valor padrão é `postgres`
* `PGADMIN_DEFAULT_EMAIL`: o valor padrão é `pgadmin@pgadmin.com`
* `PGADMIN_DEFAULT_PASSWORD`: o valor padrão é `pgadmin`

### Acesso ao Postgres

* `localhost:5432`
* **Username**: `postgres`
* **Password** `secret`

### Acesso ao PgAdmin

* Aguardar aproximadamente 5 minutos para terminar a execução do servidor
    * Pode-se verificar no Docker Desktop em Inspect.
* **URL Web App**: `http://localhost:80`
* **Username**: `pgadmin@pgadmin.com`
* **Password**: `pgadmin`
* Adicionar um novo servidor:
    * **Host name/Address**: `pgdb`  ??
    * **Port**: `5432`
    * **Username** as `POSTGRES_USER`, by default: `postgres`
    * **Password** as `POSTGRES_PASSWORD`, by default `secret`