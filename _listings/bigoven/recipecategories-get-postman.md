{
  "info": {
    "name": "Big Oven Get a list of recipe categories (the ID field can be used for include_cat in search parameters)",
    "_postman_id": "3d75f006-c5c2-4ac5-803f-0f875aa1ab42",
    "description": "Get a list of recipe categories (the id field can be used for include_cat in search parameters).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "c1ee4669-e204-4fa9-aab5-2529512f0300",
          "name": "Recipe_Categories",
          "request": {
            "url": "http://api2.bigoven.com/recipe/categories",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of recipe categories (the id field can be used for include_cat in search parameters)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c042b271-0a3d-4454-8dc0-88cf1dda7bff"
            }
          ]
        }
      ]
    }
  ]
}