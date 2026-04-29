# Clientes API

API REST para gerenciamento de clientes, desenvolvida com Java e Spring Boot.

## Tecnologias

- Java
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Docker

## Como rodar

**1. Suba o banco de dados:**

```bash
docker-compose up -d
```

**2. Suba o servidor:**

```bash
.\mvnw.cmd spring-boot:run
```

A API estará disponível em `http://localhost:8080`.

## Endpoints

| Método | URL | Descrição |
|--------|-----|-----------|
| GET | /clientes | Lista todos os clientes |
| GET | /clientes/{id} | Busca um cliente pelo id |
| POST | /clientes | Cria um novo cliente |
| PUT | /clientes/{id} | Atualiza um cliente |
| DELETE | /clientes/{id} | Deleta um cliente |

## Exemplo de requisição

```json
{
    "nome": "João Silva",
    "email": "joao@email.com",
    "telefone": "47999998888"
}
```