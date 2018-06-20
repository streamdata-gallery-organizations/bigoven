---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: Big Oven Gets a recipe collection metadata. A recipe collection is a curated
    set of recipes.
  description: Gets a recipe collection metadata. a recipe collection is a curated
    set of recipes..
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