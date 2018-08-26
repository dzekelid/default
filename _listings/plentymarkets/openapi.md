---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/{id}/variations/{variationId}/variation_default_categories:
    get:
      summary: List default category links
      description: Lists the default category of a variation for all clients (stores).
        The ID of the item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Default
      - Category
      - Links
    post:
      summary: Create a default category link
      description: Creates a link between a variation and a category that designates
        the category as the default category.
      operationId: postRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_default_categories/{plentyId}:
    delete:
      summary: Delete a default category link
      description: Deletes a link between a variation and a category that designates
        this category as the default category.
      operationId: deleteRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
    get:
      summary: Gets a default category link
      description: Gets the default category linked to a variation for the specified
        client (store). The ID of the item, the ID of the variation and the ID of
        the client (store) must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Default
      - Category
      - Link
---