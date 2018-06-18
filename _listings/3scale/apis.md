---
name: 3scale
x-slug: 3scale
description: 3scales API Management platform gives you the tools you need to take
  control of your API. Trusted by more customers than any other vendor.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
x-kinRank: "10"
x-alexaRank: "345437"
tags: Default
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/3scale/apis.md
specificationVersion: "0.14"
apis:
- name: 3Scale Account Management API Account Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: Account plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/account_plans/{id}/default.xml
  tags: Account,Plan,Set,To,Default
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/3scale/adminapiaccount-plansiddefault-xml-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/3scale/adminapiaccount-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API Application Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: Application plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/application_plans/{id}/default.xml
  tags: Application,Plan,Set,To,Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/3scale/adminapiservicesservice-idapplication-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API End User Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: End user plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/end_user_plans/{id}/default.xml
  tags: End,User,Plan,Set,To,Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/3scale/adminapiservicesservice-idend-user-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API Service Plan set to Default
  x-api-slug: 3scale-account-management-api
  description: Service plan set to default.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net////admin/api/services/{service_id}/service_plans/{id}/default.xml
  tags: Service,Plan,Set,To,Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/3scale/adminapiservicesservice-idservice-plansiddefault-xml-put-openapi.md
- name: 3Scale Account Management API
  x-api-slug: 3scale-account-management-api
  description: 3scales API Management platform gives you the tools you need to take
    control of your API. Trusted by more customers than any other vendor.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/4-3scale.jpg
  humanURL: http://3scale.net
  baseURL: https://su1.3scale.net//
  tags: Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/3scale/openapi.md
x-common:
- type: x-blog
  url: http://www.3scale.net/blog/
- type: x-blog-rss
  url: http://www.3scale.net/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/3scale
- type: x-crunchbase
  url: https://crunchbase.com/organization/3scale
- type: x-email
  url: sales@3scale.net
- type: x-email
  url: info@3scale.net
- type: x-github
  url: https://github.com/3scale
- type: x-pricing
  url: https://www.3scale.net/pricing/
- type: x-privacy
  url: https://www.3scale.net/privacy-policy/
- type: x-support
  url: https://support.3scale.net
- type: x-openapi-spec
  url: https://support.3scale.net/reference/active-docs
- type: x-terms-of-service
  url: https://www.3scale.net/terms-and-conditions/
- type: x-twitter
  url: https://twitter.com/3scale
- type: x-website
  url: http://3scale.net
- type: x-website
  url: http://
- type: x-website
  url: http://www.3scale.net
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---