{
  "info": {
    "name": "Big Oven Get the user's grocery list.  User is determined by Basic Authentication.",
    "_postman_id": "e84f3184-87a1-40cf-a588-08c15883b54b",
    "description": "Get the user's grocery list.  user is determined by basic authentication..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Recipes",
      "item": [
        {
          "id": "8f6a8fdc-7461-471d-980e-4ea59fe3a18e",
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
              "id": "54837b55-c9c8-4911-8af8-b1466e366428"
            }
          ]
        },
        {
          "id": "b0292823-67b7-4b30-9c5c-0b6a4f8defd8",
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
              "id": "d207fc95-346e-4689-b7ee-939bcc145909"
            }
          ]
        },
        {
          "id": "7a11a70d-a32f-40f9-8116-eda43b3f3030",
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
              "id": "826a5dd6-2238-4607-855d-d7edda1528b6"
            }
          ]
        },
        {
          "id": "825aaad4-649c-4204-a6a5-d80ec743425f",
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
              "id": "9bd7f717-45c7-4765-bff9-af642720b3e7"
            }
          ]
        },
        {
          "id": "5b4a1fb2-985f-4b60-8613-05ff1d67eb6c",
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
              "id": "ec6d675e-fc0a-480b-b125-c72fe46c61ec"
            }
          ]
        },
        {
          "id": "e0db910a-dd05-4e70-8da6-29e666f3f600",
          "name": "GroceryList_Get",
          "request": {
            "url": "http://api2.bigoven.com/grocerylist",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the user's grocery list.  user is determined by basic authentication.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "613f6a7e-87f3-4464-a81b-75f4a0ca8cdc"
            }
          ]
        },
        {
          "id": "b76f5da7-40c5-42f1-8ab1-aab0b6550e45",
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
              "id": "6338d04d-1ed3-4c59-aa90-1003adfc7f87"
            }
          ]
        }
      ]
    }
  ]
}