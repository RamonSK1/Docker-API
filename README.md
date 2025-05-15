# API de Receitas

Este projeto é uma API RESTful desenvolvida com **Flask** que permite realizar o CRUD (Criar, Ler, Atualizar e Deletar) de **ingredientes** e **receitas**. Cada receita pode conter múltiplos ingredientes com suas respectivas quantidades e um modo de preparo. Porem agora implementadada com Dockers

---

## Funcionalidades

- CRUD de ingredientes
- CRUD de receitas
- Associação de ingredientes a receitas com quantidade
- Descrição de modo de preparo por receita

---

## Tecnologias Utilizadas

- Python
- Flask
- Flask-Migrate
- SQLAlchemy
- SQLite (padrão, pode ser substituído por outro banco)

---

## Como rodar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/RamonSK1/Docker-API.git
cd Docker-API
```
### 2. Execute o comando
docker-compose up --build (sudo se for user normal)
---

O servidor estará disponível em:
```
http://127.0.0.1:5000
```

---

## Endpoints principais

### Ingredientes
- `GET /ingredientes` — Lista todos os ingredientes
- `POST /ingredientes` — Cria um novo ingrediente
- `GET /ingredientes/<id>` — Detalha um ingrediente
- `PUT /ingredientes/<id>` — Atualiza um ingrediente
- `DELETE /ingredientes/<id>` — Deleta um ingrediente

### Receitas
- `GET /receitas` — Lista todas as receitas
- `POST /receitas` — Cria uma nova receita
- `GET /receitas/<id>` — Detalha uma receita, com ingredientes
- `PUT /receitas/<id>` — Atualiza uma receita
- `DELETE /receitas/<id>` — Deleta uma receita
- `POST /receitas/<receita_id>/ingredientes` — Adiciona ingredientes à receita


