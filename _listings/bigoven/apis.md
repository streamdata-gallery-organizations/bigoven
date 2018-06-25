---
name: BigOven
x-slug: bigoven
description: Free recipe app for home cooks. Create a meal plan, grocery list and
  more from your favorite recipes. Organize your recipe collection and take it anywhere.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
x-kinRank: "8"
x-alexaRank: "117577"
tags: BigOven
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/apis.md
specificationVersion: "0.14"
apis:
- name: Big Oven Gets a recipe collection. A recipe collection is a curated set of
    recipes.
  x-api-slug: big-oven
  description: Gets a recipe collection. a recipe collection is a curated set of recipes..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////collection/{id}
  tags: Recipes,Collection
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/collectionid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/collectionid-get-openapi.md
- name: Big Oven Gets a recipe collection metadata. A recipe collection is a curated
    set of recipes.
  x-api-slug: big-oven
  description: Gets a recipe collection metadata. a recipe collection is a curated
    set of recipes..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////collection/{id}/meta
  tags: Recipes,Collection,Meta
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/collectionidmeta-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/collectionidmeta-get-openapi.md
- name: Big Oven Get the list of current, seasonal recipe collections. From here,
    you can use the /collection/{id} endpoint to retrieve the recipes in those collections.
  x-api-slug: big-oven
  description: Get the list of current, seasonal recipe collections. from here, you
    can use the /collection/{id} endpoint to retrieve the recipes in those collections..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////collections
  tags: Recipes,Collections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/collections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/collections-get-openapi.md
- name: Big Oven Get food glossary article by term (e.g., asparagus). This editorial
    is (c) BigOven and MUST carry attribution and a link back to the glossary entry
    on BigOven.com.
  x-api-slug: big-oven
  description: Get food glossary article by term (e.g., asparagus). this editorial
    is (c) bigoven and must carry attribution and a link back to the glossary entry
    on bigoven.com..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////glossary/byterm/{term}
  tags: Recipes,Glossary,Byterm,Term
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/glossarybytermterm-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/glossarybytermterm-get-openapi.md
- name: Big Oven Get food glossary article
  x-api-slug: big-oven
  description: Get food glossary article.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////glossary/{id}
  tags: Recipes,Glossary
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/glossaryid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/glossaryid-get-openapi.md
- name: Big Oven Delete all the items on a grocery list; faster operation than a sync
    with deleted items.
  x-api-slug: big-oven
  description: Delete all the items on a grocery list; faster operation than a sync
    with deleted items..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist
  tags: Recipes,Grocerylist
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylist-delete-openapi.md
- name: Big Oven Get the user's grocery list.  User is determined by Basic Authentication.
  x-api-slug: big-oven
  description: Get the user's grocery list.  user is determined by basic authentication..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist
  tags: Recipes,Grocerylist
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylist-get-openapi.md
- name: Big Oven Departmentalize a list of strings -- used for ad-hoc grocery list
    item addition
  x-api-slug: big-oven
  description: Departmentalize a list of strings -- used for ad-hoc grocery list item
    addition.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist/department
  tags: Recipes,Grocerylist,Department
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylistdepartment-post-openapi.md
- name: Big Oven Add a single line item to the grocery list
  x-api-slug: big-oven
  description: Add a single line item to the grocery list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist/item
  tags: Recipes,Grocerylist,Item
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylistitem-post-openapi.md
- name: Big Oven /grocerylist/item/{guid}  DELETE will delete this item assuming you
    own it.
  x-api-slug: big-oven
  description: /grocerylist/item/{guid}  delete will delete this item assuming you
    own it..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist/item/{guid}
  tags: Recipes,Grocerylist,Item,Guid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylistitemguid-delete-openapi.md
- name: Big Oven Update a grocery item by GUID
  x-api-slug: big-oven
  description: Update a grocery item by guid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist/item/{guid}
  tags: Recipes,Grocerylist,Item,Guid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylistitemguid-put-openapi.md
- name: "Big Oven Add a Recipe to the grocery list.  In the request data, pass in
    recipeId, scale (scale=1.0 says to keep the recipe the same size as originally
    posted), markAsPending (true/false) to indicate that\r\n            the lines
    in the recipe should be marked"
  x-api-slug: big-oven
  description: "Add a recipe to the grocery list.  in the request data, pass in recipeid,
    scale (scale=1.0 says to keep the recipe the same size as originally posted),
    markaspending (true/false) to indicate that\r\n            the lines in the recipe
    should be marked ."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist/recipe
  tags: Recipes,Grocerylist,Recipe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylistrecipe-post-openapi.md
- name: Big Oven Synchronize the grocery list.  Call this with a POST to /grocerylist/sync
  x-api-slug: big-oven
  description: Synchronize the grocery list.  call this with a post to /grocerylist/sync.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////grocerylist/sync
  tags: Recipes,Grocerylist,Sync
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/grocerylistsync-post-openapi.md
- name: Big Oven Add a new recipe
  x-api-slug: big-oven
  description: Add a new recipe.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe
  tags: Recipes,Recipe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipe-post-openapi.md
- name: Big Oven Update a recipe
  x-api-slug: big-oven
  description: Update a recipe.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe
  tags: Recipes,Recipe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipe-put-openapi.md
- name: Big Oven Given a query, return recipe titles starting with query. Query must
    be at least 3 chars in length.
  x-api-slug: big-oven
  description: Given a query, return recipe titles starting with query. query must
    be at least 3 chars in length..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/autocomplete
  tags: Recipes,Recipe,Autocomplete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipeautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipeautocomplete-get-openapi.md
- name: Big Oven Get a list of recipe categories (the ID field can be used for include_cat
    in search parameters)
  x-api-slug: big-oven
  description: Get a list of recipe categories (the id field can be used for include_cat
    in search parameters).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/categories
  tags: Recipes,Recipe,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipecategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipecategories-get-openapi.md
- name: Big Oven DELETE a reply to a given review. Authenticated user must be the
    one who originally posted the reply.
  x-api-slug: big-oven
  description: Delete a reply to a given review. authenticated user must be the one
    who originally posted the reply..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/review/replies/{replyId}
  tags: Recipes,Recipe,Review,Replies,ReplyId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipereviewrepliesreplyid-delete-openapi.md
- name: Big Oven Update (PUT) a reply to a given review. Authenticated user must be
    the original one that posted the reply.
  x-api-slug: big-oven
  description: Update (put) a reply to a given review. authenticated user must be
    the original one that posted the reply..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/review/replies/{replyId}
  tags: Recipes,Recipe,Review,Replies,ReplyId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipereviewrepliesreplyid-put-openapi.md
- name: "Big Oven Get a given review by string-style ID. This will return a payload
    with FeaturedReply, ReplyCount.\r\n            Recommended display is to list
    top-level reviews with one featured reply underneath. \r\n            Currently,
    the FeaturedReply is the most"
  x-api-slug: big-oven
  description: "Get a given review by string-style id. this will return a payload
    with featuredreply, replycount.\r\n            recommended display is to list
    top-level reviews with one featured reply underneath. \r\n            currently,
    the featuredreply is the most."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/review/{reviewId}
  tags: Recipes,Recipe,Review,ReviewId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipereviewreviewid-get-openapi.md
- name: Big Oven Update a given top-level review.
  x-api-slug: big-oven
  description: Update a given top-level review..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/review/{reviewId}
  tags: Recipes,Recipe,Review,ReviewId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipereviewreviewid-put-openapi.md
- name: Big Oven Get a paged list of replies for a given review.
  x-api-slug: big-oven
  description: Get a paged list of replies for a given review..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/review/{reviewId}/replies
  tags: Recipes,Recipe,Review,ReviewId,Replies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipereviewreviewidreplies-get-openapi.md
- name: Big Oven POST a reply to a given review. The date will be set by server. Note
    that replies no longer have star ratings, only top-level reviews do.
  x-api-slug: big-oven
  description: Post a reply to a given review. the date will be set by server. note
    that replies no longer have star ratings, only top-level reviews do..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/review/{reviewId}/replies
  tags: Recipes,Recipe,Review,ReviewId,Replies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipereviewreviewidreplies-post-openapi.md
- name: "Big Oven POST an image as a new RecipeScan request\r\n                1)
    \ Fetch the filename -- DONE\r\n                2)  Copy it to the pics/scan folder
    - ENSURE NO NAMING COLLISIONS -- DONE\r\n                3)  Create 120 thumbnail
    size  in pics/scan/120 -- D"
  x-api-slug: big-oven
  description: "Post an image as a new recipescan request\r\n                1)  fetch
    the filename -- done\r\n                2)  copy it to the pics/scan folder -
    ensure no naming collisions -- done\r\n                3)  create 120 thumbnail
    size  in pics/scan/120 -- d."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/scan
  tags: Recipes,Recipe,Scan
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipescan-post-openapi.md
- name: Big Oven Delete a Recipe (you must be authenticated as an owner of the recipe)
  x-api-slug: big-oven
  description: Delete a recipe (you must be authenticated as an owner of the recipe).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{id}
  tags: Recipes,Recipe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipeid-delete-openapi.md
- name: Big Oven Return full Recipe detail. Returns 403 if the recipe is owned by
    someone else.
  x-api-slug: big-oven
  description: Return full recipe detail. returns 403 if the recipe is owned by someone
    else..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{id}
  tags: Recipes,Recipe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipeid-get-openapi.md
- name: Big Oven Feedback on a Recipe -- for internal BigOven editors
  x-api-slug: big-oven
  description: Feedback on a recipe -- for internal bigoven editors.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/feedback
  tags: Recipes,Recipe,RecipeId,Feedback
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidfeedback-post-openapi.md
- name: "Big Oven POST: /recipe/{recipeId}/image?lat=42&amp;lng=21&amp;caption=this%20is%20my%20caption\r\n
    \            \r\n             Note that caption, lng and lat are all optional,
    but must go on the request URI as params because this endpoint\r\n             needs
    a m"
  x-api-slug: big-oven
  description: "Post: /recipe/{recipeid}/image?lat=42&amp;lng=21&amp;caption=this%20is%20my%20caption\r\n
    \            \r\n             note that caption, lng and lat are all optional,
    but must go on the request uri as params because this endpoint\r\n             needs
    a m."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/image
  tags: Recipes,Recipe,RecipeId,Image
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidimage-post-openapi.md
- name: Big Oven Get all the images for a recipe. DEPRECATED. Please use /recipe/{recipeId}/photos.
  x-api-slug: big-oven
  description: Get all the images for a recipe. deprecated. please use /recipe/{recipeid}/photos..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/images
  tags: Recipes,Recipe,RecipeId,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidimages-get-openapi.md
- name: Big Oven HTTP POST a new note into the system.
  x-api-slug: big-oven
  description: Http post a new note into the system..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/note
  tags: Recipes,Recipe,RecipeId,Note
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidnote-post-openapi.md
- name: "Big Oven Delete a review\r\n                do a DELETE Http request of /note/{ID}"
  x-api-slug: big-oven
  description: "Delete a review\r\n                do a delete http request of /note/{id}."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/note/{noteId}
  tags: Recipes,Recipe,RecipeId,Note,NoteId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidnotenoteid-delete-openapi.md
- name: Big Oven Get a given note. Make sure you're passing authentication information
    in the header for the user who owns the note.
  x-api-slug: big-oven
  description: Get a given note. make sure you're passing authentication information
    in the header for the user who owns the note..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/note/{noteId}
  tags: Recipes,Recipe,RecipeId,Note,NoteId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidnotenoteid-get-openapi.md
- name: Big Oven HTTP PUT (update) a Recipe note (RecipeNote).
  x-api-slug: big-oven
  description: Http put (update) a recipe note (recipenote)..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/note/{noteId}
  tags: Recipes,Recipe,RecipeId,Note,NoteId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidnotenoteid-put-openapi.md
- name: Big Oven recipe/100/notes
  x-api-slug: big-oven
  description: Recipe/100/notes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/notes
  tags: Recipes,Recipe,RecipeId,Notes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidnotes-get-openapi.md
- name: Big Oven Get all the photos for a recipe
  x-api-slug: big-oven
  description: Get all the photos for a recipe.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/photos
  tags: Recipes,Recipe,RecipeId,Photos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidphotos-get-openapi.md
- name: Big Oven Get recipes related to the given recipeId
  x-api-slug: big-oven
  description: Get recipes related to the given recipeid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/related
  tags: Recipes,Recipe,RecipeId,Related
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidrelated-get-openapi.md
- name: Big Oven Get *my* review for the recipe {recipeId}, where "me" is determined
    by standard authentication headers
  x-api-slug: big-oven
  description: Get *my* review for the recipe {recipeid}, where "me" is determined
    by standard authentication headers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/review
  tags: Recipes,Recipe,RecipeId,Review
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidreview-get-openapi.md
- name: Big Oven Add a new review. Only one review can be provided per {userId, recipeId}
    pair. Otherwise your review will be updated.
  x-api-slug: big-oven
  description: Add a new review. only one review can be provided per {userid, recipeid}
    pair. otherwise your review will be updated..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/review
  tags: Recipes,Recipe,RecipeId,Review
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidreview-post-openapi.md
- name: "Big Oven Delete a review by recipeId and reviewId. DEPRECATED. Please see
    recipe/review/{reviewId} for the preferred method.\r\n            (We are moving
    from an integer-based ID system to a GUID-style string-based ID system for reviews
    and replies.)"
  x-api-slug: big-oven
  description: "Delete a review by recipeid and reviewid. deprecated. please see recipe/review/{reviewid}
    for the preferred method.\r\n            (we are moving from an integer-based
    id system to a guid-style string-based id system for reviews and replies.)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/review/{reviewId}
  tags: Recipes,Recipe,RecipeId,Review,ReviewId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidreviewreviewid-delete-openapi.md
- name: "Big Oven Get a given review - DEPRECATED. See recipe/review/{reviewId} for
    the current usage.\r\n            Beginning in January 2017, BigOven moded from
    an integer-based ID system to a GUID-style string-based ID system for reviews
    and replies.\r\n            We"
  x-api-slug: big-oven
  description: "Get a given review - deprecated. see recipe/review/{reviewid} for
    the current usage.\r\n            beginning in january 2017, bigoven moded from
    an integer-based id system to a guid-style string-based id system for reviews
    and replies.\r\n            we."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/review/{reviewId}
  tags: Recipes,Recipe,RecipeId,Review,ReviewId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidreviewreviewid-get-openapi.md
- name: "Big Oven HTTP PUT (update) a recipe review. DEPRECATED. Please see recipe/review/{reviewId}
    PUT for the new endpoint.\r\n            We are moving to a string-based primary
    key system, no longer integers, for reviews and replies."
  x-api-slug: big-oven
  description: "Http put (update) a recipe review. deprecated. please see recipe/review/{reviewid}
    put for the new endpoint.\r\n            we are moving to a string-based primary
    key system, no longer integers, for reviews and replies.."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/review/{reviewId}
  tags: Recipes,Recipe,RecipeId,Review,ReviewId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidreviewreviewid-put-openapi.md
- name: Big Oven Get paged list of reviews for a recipe. Each review will have at
    most one FeaturedReply, as well as a ReplyCount.
  x-api-slug: big-oven
  description: Get paged list of reviews for a recipe. each review will have at most
    one featuredreply, as well as a replycount..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/reviews
  tags: Recipes,Recipe,RecipeId,Reviews
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidreviews-get-openapi.md
- name: Big Oven Gets a list of RecipeScan images for the recipe. There will be at
    most 3 per recipe.
  x-api-slug: big-oven
  description: Gets a list of recipescan images for the recipe. there will be at most
    3 per recipe..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipe/{recipeId}/scans
  tags: Recipes,Recipe,RecipeId,Scans
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/reciperecipeidscans-get-openapi.md
- name: "Big Oven Search for recipes. There are many parameters that you can apply.
    Starting with the most common, use title_kw to search within a title.\r\n            Use
    any_kw to search across the entire recipe.\r\n            If you'd like to limit
    by course, set the"
  x-api-slug: big-oven
  description: "Search for recipes. there are many parameters that you can apply.
    starting with the most common, use title_kw to search within a title.\r\n            use
    any_kw to search across the entire recipe.\r\n            if you'd like to limit
    by course, set the."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipes
  tags: Recipes,Recipes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipes-get-openapi.md
- name: Big Oven Get a random, home-page-quality Recipe.
  x-api-slug: big-oven
  description: Get a random, home-page-quality recipe..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipes/random
  tags: Recipes,Recipes,Random
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipesrandom-get-openapi.md
- name: Big Oven Get the recipe/comment tuples for those recipes with 4 or 5 star
    ratings
  x-api-slug: big-oven
  description: Get the recipe/comment tuples for those recipes with 4 or 5 star ratings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipes/raves
  tags: Recipes,Recipes,Raves
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipesraves-get-openapi.md
- name: Big Oven Get a list of recipes that the authenticated user has most recently
    viewed
  x-api-slug: big-oven
  description: Get a list of recipes that the authenticated user has most recently
    viewed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com////recipes/recentviews
  tags: Recipes,Recipes,Recentviews
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/recipesrecentviews-get-openapi.md
- name: Big Oven
  x-api-slug: big-oven
  description: Free recipe app for home cooks. Create a meal plan, grocery list and
    more from your favorite recipes. Organize your recipe collection and take it anywhere.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/379-bigoven.jpg
  humanURL: http://www.bigoven.com
  baseURL: https://api2.bigoven.com//
  tags: BigOven
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bigoven/master/_listings/bigoven/openapi.md
x-common:
- type: x-website
  url: http://www.bigoven.com
- type: x-base
  url: http://api.bigoven.com/
- type: x-blog
  url: http://blog.bigoven.com/
- type: x-blog-rss
  url: http://blog.bigoven.com/index.php/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/bigoven
- type: x-crunchbase
  url: http://www.crunchbase.com/company/bigoven
- type: x-developer
  url: http://api.bigoven.com
- type: x-documentation
  url: http://api2.bigoven.com/
- type: x-email
  url: support@bigoven.com
- type: x-twitter
  url: https://twitter.com/bigoven
- type: x-website
  url: http://bigoven.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---