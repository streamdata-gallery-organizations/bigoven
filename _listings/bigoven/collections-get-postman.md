{
  "info": {
    "name": "Big Oven Get the list of current, seasonal recipe collections. From here, you can use the /collection/{id} endpoint to retrieve the recipes in those collections.",
    "_postman_id": "d1061271-1964-40db-80fa-1b3d77b9d199",
    "description": "Get the list of current, seasonal recipe collections. from here, you can use the /collection/{id} endpoint to retrieve the recipes in those collections..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "1bb07cab-446f-492a-805d-287a6952cc23",
          "name": "Collection_Collections",
          "request": {
            "url": "http://api2.bigoven.com/collections?test=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of current, seasonal recipe collections. from here, you can use the /collection/{id} endpoint to retrieve the recipes in those collections.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6fbe36b-f570-477e-9617-a8c62d5f413d"
            }
          ]
        }
      ]
    }
  ]
}