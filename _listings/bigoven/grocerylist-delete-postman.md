{
  "info": {
    "name": "Big Oven Delete all the items on a grocery list; faster operation than a sync with deleted items.",
    "_postman_id": "7f7ac834-4bad-406d-8bd9-3879b2be9771",
    "description": "Delete all the items on a grocery list; faster operation than a sync with deleted items..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "99794e6f-d515-45a1-aa5a-c2d4027beb83",
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
              "id": "3ef37e70-e142-49f5-86e2-88b408171b60"
            }
          ]
        },
        {
          "id": "7c3f674f-e06e-43e4-8d6e-23e150abaa46",
          "name": "Collection_GetCollectionMeta",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "collection/:id/meta"
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
            "description": "Gets a recipe collection metadata. a recipe collection is a curated set of recipes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f340cc54-f505-4adb-8c05-97046fd7dbf9"
            }
          ]
        },
        {
          "id": "a61c2cd7-af47-4ba7-a3a2-19b62bab65c7",
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
              "id": "ce3a2ac1-8333-4b63-bef7-0d92d17e0c10"
            }
          ]
        },
        {
          "id": "43ae32c3-db47-4603-adff-19ba8644d738",
          "name": "Glossary_ByTerm",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "glossary/byterm/:term"
              ],
              "variable": [
                {
                  "id": "term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get food glossary article by term (e.g., asparagus). this editorial is (c) bigoven and must carry attribution and a link back to the glossary entry on bigoven.com.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39b93038-393e-4a08-a9bd-77c36d1d24d2"
            }
          ]
        },
        {
          "id": "e53df55a-d252-4160-beb7-235e635cd634",
          "name": "Glossary_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.bigoven.com",
              "path": [
                "glossary/:id"
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
            "description": "Get food glossary article."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f46a960d-7d9b-4da4-9626-c10bd5e6497b"
            }
          ]
        },
        {
          "id": "d4ff280a-70b5-4e3c-a4ec-62f9bc97d2f6",
          "name": "GroceryList_Delete",
          "request": {
            "url": "http://api2.bigoven.com/grocerylist",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete all the items on a grocery list; faster operation than a sync with deleted items.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce1ab197-daff-4897-85ee-594a966d69eb"
            }
          ]
        }
      ]
    }
  ]
}