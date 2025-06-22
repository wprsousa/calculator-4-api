# 🧮 Calculator 4 - Desafio 04 | Rocketseat

Este projeto é uma solução para o **Desafio 04** do módulo **Introdução ao Design de Código** da trilha da Rocketseat.

A aplicação consiste na criação de uma rota chamada `calculator_4` que recebe uma lista de números via requisição `POST` e retorna a **média aritmética** desses números. O projeto foi desenvolvido com foco em boas práticas de design de código.

---

## 🚀 Tecnologias Utilizadas

- Python 3.11+
- Flask
- pytest
- Estrutura modular com separação de responsabilidades

---

## ⚙️ Funcionalidades

- 📥 Receber uma lista de números em uma requisição POST
- 📊 Calcular e retornar a média aritmética
- 🔒 Validação e tratamento de erro para payloads inválidos
- ✅ Testes automatizados com cobertura das funcionalidades principais
- 📁 Código organizado em arquivos e módulos separados

---

## 📁 Estrutura do Projeto

```text
.
├── app/
│   ├── routes/
│   │   └── calculator_4.py
│   ├── services/
│   │   └── average_service.py
│   └── __init__.py
├── tests/
│   └── test_calculator_4.py
├── run.py
├── requirements.txt
└── README.md
```

---

## 🧰 Como executar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/calculator-4-api.git
cd calculator-4-api
```

### 2. Crie e ative um ambiente virtual

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

### 4. Rode o servidor Flask

```bash
flask --app run run
```

---

## 📮 Exemplo de requisição

### POST `/calculator_4`

**Body (JSON):**

```json
{
  "numbers": [10, 20, 30, 40]
}
```

**Resposta esperada:**

```json
{
  "average": 25.0
}
```

### Caso envie dados incorretos:

```json
{
  "error": "O campo 'numbers' deve ser uma lista de números válidos."
}
```

---

## 🧪 Executando os Testes

```bash
pytest
```

---

## 💭 Aprendizados

Durante este desafio, foram reforçados os seguintes pontos:

- Boas práticas de design de código em Flask
- Organização modular por responsabilidades
- Validação de entradas e tratamento de erros
- Especificação e criação de testes automatizados

---

## 📌 Entrega

URL do projeto: [https://github.com/seu-usuario/calculator-4-api](https://github.com/seu-usuario/calculator-4-api)

---

## 🧑‍💻 Autor

Feito com 💜 por [Seu Nome](https://github.com/seu-usuario) para o desafio da Rocketseat.
