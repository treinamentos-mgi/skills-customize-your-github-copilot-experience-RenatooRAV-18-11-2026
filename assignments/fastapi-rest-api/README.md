# 📘 Atividade: Building REST APIs with FastAPI framework

## 🎯 Objetivo

Construa uma API REST introdutória com FastAPI e pratique rotas HTTP, validação de dados com Pydantic e operações CRUD usando armazenamento em memória.

## 📝 Tarefas

### 🛠️ Criar a aplicação FastAPI

#### Descrição

Configure uma aplicação FastAPI em `main.py` e crie endpoints iniciais para apresentar a API e listar itens. Execute a aplicação localmente com Uvicorn.

#### Requisitos
O programa concluído deve:

- Criar uma instância da aplicação FastAPI em `main.py`.
- Disponibilizar `GET /` e retornar uma mensagem em formato JSON.
- Disponibilizar `GET /items` e retornar uma lista JSON, vazia quando não houver itens.
- Permitir acesso à documentação interativa gerada pelo FastAPI em `/docs`.

### 🛠️ Implementar operações CRUD para itens

#### Descrição

Defina um modelo de item com Pydantic e implemente operações para criar, consultar, atualizar e remover itens. Mantenha os dados em memória durante a execução da aplicação; não é necessário configurar um banco de dados.

#### Requisitos
O programa concluído deve:

- Definir um modelo de item com um nome obrigatório e uma descrição opcional.
- Disponibilizar `POST /items` para criar um item e retornar o item criado com status HTTP `201`.
- Disponibilizar `GET /items/{item_id}` para consultar um item pelo identificador.
- Disponibilizar `PUT /items/{item_id}` para atualizar um item existente.
- Disponibilizar `DELETE /items/{item_id}` para remover um item existente e retornar status HTTP `204`.
- Retornar status HTTP `404` quando uma operação solicitar um item inexistente.
- Rejeitar dados de entrada inválidos usando a validação do Pydantic.
