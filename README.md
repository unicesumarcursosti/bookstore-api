# 📘 Exercício: Sistema de Livraria - Cadastro de Livros (Spring Boot + Collections)

## 🎯 Objetivo

Construir uma API REST utilizando **Spring Boot**, capaz de realizar operações básicas de **cadastro, listagem e consulta de livros**, utilizando apenas **Collections em memória**.

---

## 🧱 Requisitos Funcionais

1. Permitir o **cadastro de um livro**, contendo as seguintes informações:
   - `título` (obrigatório)
   - `autor` (obrigatório)
   - `ano de publicação`
   - `ISBN`
   - O sistema deve gerar um **ID único** automaticamente para cada livro cadastrado.
   Corpo da requisição (JSON):
```json
{
  "titulo": "O Senhor dos Anéis",
  "autor": "J.R.R. Tolkien",
  "anoPublicacao": 1954,
  "isbn": "978-0544003415"
}

```

2. Permitir a **listagem de todos os livros cadastrados**.

3. Permitir a **consulta de um livro individual** a partir de seu ID.

4. Permitir a **remoção de um livro** a partir do ID.

---

## 🧠 Regras e Restrições

- **Não utilizar JPA, Hibernate ou qualquer banco de dados**.
- Os dados dos livros devem ser armazenados em memória usando **Java Collections**, como `List` ou `Map`.
- A aplicação deve seguir a estrutura de pacotes organizada em:
  - `model` – para a classe `Livro`
  - `controller` – para o controle das requisições HTTP
