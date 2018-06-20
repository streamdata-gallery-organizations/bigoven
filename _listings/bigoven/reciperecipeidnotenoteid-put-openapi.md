---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: Big Oven HTTP PUT (update) a Recipe note (RecipeNote).
  description: Http put (update) a recipe note (recipenote)..
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
  /recipe:
    post:
      summary: Add a new recipe
      description: Add a new recipe.
      operationId: Recipe_Post
      x-api-path-slug: recipe-post
      parameters:
      - in: body
        name: recipe
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
    put:
      summary: Update a recipe
      description: Update a recipe.
      operationId: Recipe_Put
      x-api-path-slug: recipe-put
      parameters:
      - in: body
        name: recipe
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
  /recipe/autocomplete:
    get:
      summary: Given a query, return recipe titles starting with query. Query must
        be at least 3 chars in length.
      description: Given a query, return recipe titles starting with query. query
        must be at least 3 chars in length..
      operationId: Recipe_AutoComplete
      x-api-path-slug: recipeautocomplete-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Autocomplete
  /recipe/categories:
    get:
      summary: Get a list of recipe categories (the ID field can be used for include_cat
        in search parameters)
      description: Get a list of recipe categories (the id field can be used for include_cat
        in search parameters).
      operationId: Recipe_Categories
      x-api-path-slug: recipecategories-get
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Categories
  /recipe/review/replies/{replyId}:
    delete:
      summary: DELETE a reply to a given review. Authenticated user must be the one
        who originally posted the reply.
      description: Delete a reply to a given review. authenticated user must be the
        one who originally posted the reply..
      operationId: Review_DeleteReply
      x-api-path-slug: recipereviewrepliesreplyid-delete
      parameters:
      - in: path
        name: replyId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - Replies
      - ReplyId
    put:
      summary: Update (PUT) a reply to a given review. Authenticated user must be
        the original one that posted the reply.
      description: Update (put) a reply to a given review. authenticated user must
        be the original one that posted the reply..
      operationId: Review_PutReply
      x-api-path-slug: recipereviewrepliesreplyid-put
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: replyId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - Replies
      - ReplyId
  /recipe/review/{reviewId}:
    get:
      summary: "Get a given review by string-style ID. This will return a payload
        with FeaturedReply, ReplyCount.\r\n            Recommended display is to list
        top-level reviews with one featured reply underneath. \r\n            Currently,
        the FeaturedReply is the most"
      description: "Get a given review by string-style id. this will return a payload
        with featuredreply, replycount.\r\n            recommended display is to list
        top-level reviews with one featured reply underneath. \r\n            currently,
        the featuredreply is the most."
      operationId: ""
      x-api-path-slug: recipereviewreviewid-get
      parameters:
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
    put:
      summary: Update a given top-level review.
      description: Update a given top-level review..
      operationId: Review_Put
      x-api-path-slug: recipereviewreviewid-put
      parameters:
      - in: body
        name: review
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
  /recipe/review/{reviewId}/replies:
    get:
      summary: Get a paged list of replies for a given review.
      description: Get a paged list of replies for a given review..
      operationId: Review_GetReplies
      x-api-path-slug: recipereviewreviewidreplies-get
      parameters:
      - in: query
        name: pg
        description: the page (int), starting with 1
      - in: path
        name: reviewId
      - in: query
        name: rpp
        description: results per page (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
      - Replies
    post:
      summary: POST a reply to a given review. The date will be set by server. Note
        that replies no longer have star ratings, only top-level reviews do.
      description: Post a reply to a given review. the date will be set by server.
        note that replies no longer have star ratings, only top-level reviews do..
      operationId: Review_PostReply
      x-api-path-slug: recipereviewreviewidreplies-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
      - Replies
  /recipe/scan:
    post:
      summary: "POST an image as a new RecipeScan request\r\n                1)  Fetch
        the filename -- DONE\r\n                2)  Copy it to the pics/scan folder
        - ENSURE NO NAMING COLLISIONS -- DONE\r\n                3)  Create 120 thumbnail
        size  in pics/scan/120 -- D"
      description: "Post an image as a new recipescan request\r\n                1)
        \ fetch the filename -- done\r\n                2)  copy it to the pics/scan
        folder - ensure no naming collisions -- done\r\n                3)  create
        120 thumbnail size  in pics/scan/120 -- d."
      operationId: Recipe_Scan
      x-api-path-slug: recipescan-post
      parameters:
      - in: query
        name: devicetype
      - in: query
        name: lat
      - in: query
        name: lng
      - in: query
        name: test
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Scan
  /recipe/{id}:
    delete:
      summary: Delete a Recipe (you must be authenticated as an owner of the recipe)
      description: Delete a recipe (you must be authenticated as an owner of the recipe).
      operationId: Recipe_Delete
      x-api-path-slug: recipeid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
    get:
      summary: Return full Recipe detail. Returns 403 if the recipe is owned by someone
        else.
      description: Return full recipe detail. returns 403 if the recipe is owned by
        someone else..
      operationId: Recipe_Get
      x-api-path-slug: recipeid-get
      parameters:
      - in: path
        name: id
        description: the Recipe ID to retrieve
      - in: query
        name: prefetch
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
  /recipe/{recipeId}/feedback:
    post:
      summary: Feedback on a Recipe -- for internal BigOven editors
      description: Feedback on a recipe -- for internal bigoven editors.
      operationId: Recipe_Feedback
      x-api-path-slug: reciperecipeidfeedback-post
      parameters:
      - in: body
        name: data
        description: The payload for feedback, which includes the field feedback
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: recipeId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Feedback
  /recipe/{recipeId}/image:
    post:
      summary: "POST: /recipe/{recipeId}/image?lat=42&amp;lng=21&amp;caption=this%20is%20my%20caption\r\n
        \            \r\n             Note that caption, lng and lat are all optional,
        but must go on the request URI as params because this endpoint\r\n             needs
        a m"
      description: "Post: /recipe/{recipeid}/image?lat=42&amp;lng=21&amp;caption=this%20is%20my%20caption\r\n
        \            \r\n             note that caption, lng and lat are all optional,
        but must go on the request uri as params because this endpoint\r\n             needs
        a m."
      operationId: Images_UploadRecipeImage
      x-api-path-slug: reciperecipeidimage-post
      parameters:
      - in: query
        name: caption
      - in: query
        name: lat
      - in: query
        name: lng
      - in: path
        name: recipeId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Image
  /recipe/{recipeId}/images:
    get:
      summary: Get all the images for a recipe. DEPRECATED. Please use /recipe/{recipeId}/photos.
      description: Get all the images for a recipe. deprecated. please use /recipe/{recipeid}/photos..
      operationId: Images_Get
      x-api-path-slug: reciperecipeidimages-get
      parameters:
      - in: path
        name: recipeId
        description: Recipe ID (required)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Images
  /recipe/{recipeId}/note:
    post:
      summary: HTTP POST a new note into the system.
      description: Http post a new note into the system..
      operationId: Note_Post
      x-api-path-slug: reciperecipeidnote-post
      parameters:
      - in: body
        name: note
        description: 'a recipe note, with fields: Date (YYYY-MM-DD string), Notes
          (string), People (string), Variations (string), RecipeID (int?)'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: recipeId
        description: recipeId (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
  /recipe/{recipeId}/note/{noteId}:
    delete:
      summary: "Delete a review\r\n                do a DELETE Http request of /note/{ID}"
      description: "Delete a review\r\n                do a delete http request of
        /note/{id}."
      operationId: Note_Delete
      x-api-path-slug: reciperecipeidnotenoteid-delete
      parameters:
      - in: path
        name: noteId
        description: noteId (int)
      - in: path
        name: recipeId
        description: recipeId (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
      - NoteId
    get:
      summary: Get a given note. Make sure you're passing authentication information
        in the header for the user who owns the note.
      description: Get a given note. make sure you're passing authentication information
        in the header for the user who owns the note..
      operationId: Note_Get
      x-api-path-slug: reciperecipeidnotenoteid-get
      parameters:
      - in: path
        name: noteId
        description: The note ID (note -- its not the RecipeID)
      - in: path
        name: recipeId
        description: recipe identifier (integer)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
      - NoteId
    put:
      summary: HTTP PUT (update) a Recipe note (RecipeNote).
      description: Http put (update) a recipe note (recipenote)..
      operationId: Note_Put
      x-api-path-slug: reciperecipeidnotenoteid-put
      parameters:
      - in: path
        name: noteId
      - in: path
        name: recipeId
      - in: body
        name: recipeNote
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
      - NoteId
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