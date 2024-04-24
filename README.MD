# API de Gerenciamento de Usuários

Esta é uma API simples de gerenciamento de usuários usando Node.js, Express e PostgreSQL.

## Pré-requisitos

Certifique-se de ter o Node.js e o PostgreSQL instalados em sua máquina.

## Instalação

1. Clone este repositório.
2. Instale as dependências usando `npm install`.
3. Configure o PostgreSQL com as credenciais corretas no arquivo `app.js`.

## Configuração do Banco de Dados

Certifique-se de ter um banco de dados PostgreSQL configurado com uma tabela `usuarios` com os campos `id` (INT, PRIMARY KEY), `name` (VARCHAR), `surname` (VARCHAR), `email` (VARCHAR), `birthdate` (DATE), `age` (INT) e `sign` (VARCHAR).

## Executando o Servidor

Execute o servidor usando `npm start`. Por padrão, ele estará disponível em `http://localhost:3000`.

## Endpoints Disponíveis

- `GET /usuarios`: Retorna todos os usuários cadastrados.
- `GET /usuarios/:id`: Retorna um usuário específico com base no ID.
- `POST /usuarios`: Adiciona um novo usuário.
- `PUT /usuarios/:id`: Atualiza as informações de um usuário existente.
- `DELETE /usuarios/:id`: Deleta um usuário existente.

## Exemplo de Uso

### GET /usuarios

Retorna todos os usuários cadastrados.

```bash
curl http://localhost:3000/usuarios
