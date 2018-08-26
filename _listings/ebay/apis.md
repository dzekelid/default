---
name: eBay
x-slug: ebay
description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
  goods, digital cameras, baby items, coupons, and everything else on eBay, the worlds
  online marketplace
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
x-kinRank: "8"
x-alexaRank: "42"
tags: Default
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/ebay/apis.md
specificationVersion: "0.14"
apis:
- name: Ebay - Get Get Default Category Tree
  x-api-slug: get-default-category-tree-id-get
  description: A given eBay marketplace might use multiple category trees, but one
    of those trees is considered to be the default for that marketplace. This call
    retrieves a reference to the default category tree associated with the specified
    eBay marketplace ID. The response includes only the tree's unique identifier and
    version, which you can use to retrieve more details about the tree, its structure,
    and its individual category nodes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/ebay/get-default-category-tree-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/ebay/get-default-category-tree-id-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://easycron.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ebay.stack.network
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-crunchbase
  url: https://crunchbase.com/organization/leah
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-email
  url: spam@ebay.com
- type: x-email
  url: spoof@ebay.com
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/eBay
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---