# simple-code-challenge-for-juniors
Este é a descrição  de um projeto de API para lecionar programação do zero para juniores que sera devidido em etapas:

# pre work
realize o fork desse projeto para seu github

# Etapa 1
* Escolha uma linguagem de programação, nesse momento sugiro PHP, por sua simplicidade
* Crie uma imagem docker para seu projeto
* disponibilize um end-point `/probe` o qual deve responder
   *  **HttpStatus** 200
   *  **Payload** ```js {"app": "nomeDaSuaApp", "status": "OK"}```

# Etapa 2
* Disponibilizar um endpoint `/clients` onde deve responder o id, nome e o total de orders de cada cliente
* Disponibilizar um endpoint `/clients/{id}/orders` onde deve responder todas as orders realizadas por esse cliente
* utilize o json abaixo como modelo statico de dados, nesse momento não iremos necessitar de uma base de dados.

```js
{
  "id": 1,
  "name": "Eric Cartman",
  "num_orders": 2,
  "orders": [
    {
      "order_id": 1,
      "date": "2017-07-10T16:26:15",
      "items": [
        {
          "id": 845,
          "name": "Meteor Impact Survival Kit",
          "quantity": 1,
          "single_item_price": 299,
          "total_price": 299
        }
      ]
    },
    {
      "order_id": 2,
      "date": "2017-07-10T16:26:15",
      "items": [
        {
          "id": 232,
          "name": "Rubber Christmas Tree",
          "quantity": 1,
          "single_item_price": 65,
          "total_price": 65
        },
        {
          "id": 429,
          "name": "Air Guitar",
          "quantity": 4,
          "single_item_price": 9.99,
          "total_price": 39.96
        }
      ]
    }
  ]
}
```
