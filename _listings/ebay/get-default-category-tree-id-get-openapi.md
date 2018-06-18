---
swagger: "2.0"
x-collection-name: eBay
x-complete: 0
info:
  title: Ebay Get Get Default Category Tree
  description: A given eBay marketplace might use multiple category trees, but one
    of those trees is considered to be the default for that marketplace. This call
    retrieves a reference to the default category tree associated with the specified
    eBay marketplace ID. The response includes only the tree's unique identifier and
    version, which you can use to retrieve more details about the tree, its structure,
    and its individual category nodes.
  contact:
    name: eBay Inc.
  version: 1.0.0
host: api.ebay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_default_category_tree_id:
    get:
      summary: Get Get Default Category Tree
      description: A given eBay marketplace might use multiple category trees, but
        one of those trees is considered to be the default for that marketplace. This
        call retrieves a reference to the default category tree associated with the
        specified eBay marketplace ID. The response includes only the tree's unique
        identifier and version, which you can use to retrieve more details about the
        tree, its structure, and its individual category nodes.
      operationId: getDefaultCategoryTreeId
      x-api-path-slug: get-default-category-tree-id-get
      parameters:
      - in: query
        name: marketplace_id
        description: The ID of the eBay marketplace for which the category tree ID
          is being requested
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Default
      - Category
      - Tree
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