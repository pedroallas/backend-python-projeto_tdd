# backend-python-projeto_tdd

Autor: Pedro Allas

## Descrição

Store API desenvolvida com FastAPI, MongoDB (motor) e TDD (Pytest).

Esta API permite o cadastro, consulta, atualização e remoção de produtos de uma loja, utilizando uma arquitetura modular e testes automatizados desde o início do desenvolvimento.

### Tecnologias Utilizadas

- FastAPI
- MongoDB (motor)
- Pydantic
- Pytest & pytest-asyncio
- httpx

### Como configurar e rodar o projeto

1. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
2. Configure o MongoDB local e ajuste o arquivo `.env` com as URLs de conexão.
3. Execute a API:
   ```bash
   python -m uvicorn store_api.main:app --reload
   ```
4. Acesse a documentação automática em [http://localhost:8000/docs](http://localhost:8000/docs)

### Como rodar os testes

```bash
pytest
```

### Endpoints da API

- `POST /products` - Cria um novo produto
- `GET /products/{id}` - Busca produto por ID
- `GET /products` - Lista todos os produtos
- `PATCH /products/{id}` - Atualiza produto
- `DELETE /products/{id}` - Remove produto

### Repositório

[https://github.com/pedroallas/backend-python-projeto_tdd](https://github.com/pedroallas/backend-python-projeto_tdd)
