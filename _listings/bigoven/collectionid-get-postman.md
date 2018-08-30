{
  "info": {
    "name": "Big Oven Gets a recipe collection. A recipe collection is a curated set of recipes.",
    "_postman_id": "b1565749-72e0-4e3b-b1e3-c80ab91179ba",
    "description": "Gets a recipe collection. a recipe collection is a curated set of recipes..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "31199a50-3435-4f89-b2b2-65c8a88c7903",
          "name": "Collection_GetCollection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "collection/:id"
              ],
              "query": [
                {
                  "key": "pg",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rpp",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sessionForLogging",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "test",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a recipe collection. a recipe collection is a curated set of recipes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6b91b3e-be45-4a30-8acf-e542c0a6383e"
            }
          ]
        }
      ]
    }
  ]
}