GET /users

Descrição:
Retorna a lista de usuários

Request:
- Sem body

Response:
200 OK
[
  {
    "id": 1,
    "Nome": "Andre",
    "Sobrenone": "Florio"
  }
]


POST /users

Descrição:
Cria um novo usuário

Request:
{
  "nome": "Andre",
  "sobrenome": "Florio"
}

Response:
201 Created
[
  {
    "id": 2,
    "nome": "Andre",
    "sobrenome": "Florio"
  }
]
400 Bad Request
{
  "message": "Dados inválidos"
}


PUT /users

Descrição:
Atualiza todos os dados de um usuário existente.

Request:
{
  "nome": "Andre",
  "sobrenome": "Silva"
}

Response:
200 OK
[
  {
    "id": 1,
    "nome": "Andre",
    "sobrenome": "Silva"
  }
]
