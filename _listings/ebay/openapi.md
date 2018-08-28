swagger: "2.0"
x-collection-name: eBay
x-complete: 1
info:
  title: Ebay
  description: the-ebay-platform-offers-an-unprecedented-opportunity-to-build-a-new-ebay-business-or-expand-your-current-business-reach-new-customers-and-create-a-potential-new-stream-of-revenue--leverage-the-resources-of-the-ebay-developers-program-to-tap-into-the-ebay-marketplace-with-millions-of-active-users-globally-with-tools-and-services-that-meet-the-diverse-needs-of-buyers-and-sellers-
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