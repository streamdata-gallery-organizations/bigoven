{
  "info": {
    "name": "Big Oven Given a query, return recipe titles starting with query. Query must be at least 3 chars in length.",
    "_postman_id": "b58378ee-1503-4c4c-af8e-b19b63d66f64",
    "description": "Given a query, return recipe titles starting with query. query must be at least 3 chars in length..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "3e667ed4-0966-45b2-8908-4dd73d8d106a",
          "name": "Recipe_AutoComplete",
          "request": {
            "url": "http://api2.bigoven.com/recipe/autocomplete?limit=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a query, return recipe titles starting with query. query must be at least 3 chars in length.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "043db9d5-8e36-4be5-9f1b-e46175b82895"
            }
          ]
        }
      ]
    }
  ]
}