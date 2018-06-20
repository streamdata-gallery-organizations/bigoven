---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: Big Oven Synchronize the grocery list.  Call this with a POST to /grocerylist/sync
  description: Synchronize the grocery list.  call this with a post to /grocerylist/sync.
  termsOfService: Please see our [terms of service](http://api2.bigoven.com/web/documentation/termsofuse
  version: partner
host: api2.bigoven.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collection/{id}:
    get:
      summary: Gets a recipe collection. A recipe collection is a curated set of recipes.
      description: Gets a recipe collection. a recipe collection is a curated set
        of recipes..
      operationId: Collection_GetCollection
      x-api-path-slug: collectionid-get
      parameters:
      - in: path
        name: id
        description: the collection identifier
      - in: query
        name: pg
        description: page number (starting with 1)
      - in: query
        name: rpp
        description: results per page
      - in: query
        name: sessionForLogging
      - in: query
        name: test
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Collection
  /collection/{id}/meta:
    get:
      summary: Gets a recipe collection metadata. A recipe collection is a curated
        set of recipes.
      description: Gets a recipe collection metadata. a recipe collection is a curated
        set of recipes..
      operationId: Collection_GetCollectionMeta
      x-api-path-slug: collectionidmeta-get
      parameters:
      - in: path
        name: id
        description: the collection identifier
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Collection
      - Meta
  /collections:
    get:
      summary: Get the list of current, seasonal recipe collections. From here, you
        can use the /collection/{id} endpoint to retrieve the recipes in those collections.
      description: Get the list of current, seasonal recipe collections. from here,
        you can use the /collection/{id} endpoint to retrieve the recipes in those
        collections..
      operationId: Collection_Collections
      x-api-path-slug: collections-get
      parameters:
      - in: query
        name: test
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Collections
  /glossary/byterm/{term}:
    get:
      summary: Get food glossary article by term (e.g., asparagus). This editorial
        is (c) BigOven and MUST carry attribution and a link back to the glossary
        entry on BigOven.com.
      description: Get food glossary article by term (e.g., asparagus). this editorial
        is (c) bigoven and must carry attribution and a link back to the glossary
        entry on bigoven.com..
      operationId: Glossary_ByTerm
      x-api-path-slug: glossarybytermterm-get
      parameters:
      - in: path
        name: term
        description: Keyword used to look up article, e
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Glossary
      - Byterm
      - Term
  /glossary/{id}:
    get:
      summary: Get food glossary article
      description: Get food glossary article.
      operationId: Glossary_Get
      x-api-path-slug: glossaryid-get
      parameters:
      - in: path
        name: id
        description: identifier of article to retrieve
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Glossary
  /grocerylist:
    delete:
      summary: Delete all the items on a grocery list; faster operation than a sync
        with deleted items.
      description: Delete all the items on a grocery list; faster operation than a
        sync with deleted items..
      operationId: GroceryList_Delete
      x-api-path-slug: grocerylist-delete
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
    get:
      summary: Get the user's grocery list.  User is determined by Basic Authentication.
      description: Get the user's grocery list.  user is determined by basic authentication..
      operationId: GroceryList_Get
      x-api-path-slug: grocerylist-get
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
  /grocerylist/department:
    post:
      summary: Departmentalize a list of strings -- used for ad-hoc grocery list item
        addition
      description: Departmentalize a list of strings -- used for ad-hoc grocery list
        item addition.
      operationId: GroceryList_Department
      x-api-path-slug: grocerylistdepartment-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Department
  /grocerylist/item:
    post:
      summary: Add a single line item to the grocery list
      description: Add a single line item to the grocery list.
      operationId: GroceryList_Post
      x-api-path-slug: grocerylistitem-post
      parameters:
      - in: body
        name: newItem
        description: name, quantity, unit, notes, department
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
  /grocerylist/item/{guid}:
    delete:
      summary: /grocerylist/item/{guid}  DELETE will delete this item assuming you
        own it.
      description: /grocerylist/item/{guid}  delete will delete this item assuming
        you own it..
      operationId: GroceryList_DeleteItemByGuid
      x-api-path-slug: grocerylistitemguid-delete
      parameters:
      - in: path
        name: guid
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
      - Guid
    put:
      summary: Update a grocery item by GUID
      description: Update a grocery item by guid.
      operationId: GroceryList_GroceryListItemGuid
      x-api-path-slug: grocerylistitemguid-put
      parameters:
      - in: path
        name: guid
      - in: body
        name: req
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
      - Guid
  /grocerylist/recipe:
    post:
      summary: "Add a Recipe to the grocery list.  In the request data, pass in recipeId,
        scale (scale=1.0 says to keep the recipe the same size as originally posted),
        markAsPending (true/false) to indicate that\r\n            the lines in the
        recipe should be marked"
      description: "Add a recipe to the grocery list.  in the request data, pass in
        recipeid, scale (scale=1.0 says to keep the recipe the same size as originally
        posted), markaspending (true/false) to indicate that\r\n            the lines
        in the recipe should be marked ."
      operationId: GroceryList_AddRecipe
      x-api-path-slug: grocerylistrecipe-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Recipe
  /grocerylist/sync:
    post:
      summary: Synchronize the grocery list.  Call this with a POST to /grocerylist/sync
      description: Synchronize the grocery list.  call this with a post to /grocerylist/sync.
      operationId: GroceryList_PostGroceryListSync
      x-api-path-slug: grocerylistsync-post
      parameters:
      - in: body
        name: req
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Sync
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---