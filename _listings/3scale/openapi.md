---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 1
info:
  title: 3Scale Account Management API
  description: the-api-for-managing-3scale-accounts-
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/api/account_plans/{id}/default.xml:
    put:
      summary: Account Plan set to Default
      description: Account plan set to default.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Set
      - To
      - Default
  /admin/api/services/{service_id}/application_plans/{id}/default.xml:
    put:
      summary: Application Plan set to Default
      description: Application plan set to default.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Set
      - To
      - Default
  /admin/api/services/{service_id}/end_user_plans/{id}/default.xml:
    put:
      summary: End User Plan set to Default
      description: End user plan set to default.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - Set
      - To
      - Default
  /admin/api/services/{service_id}/service_plans/{id}/default.xml:
    put:
      summary: Service Plan set to Default
      description: Service plan set to default.
      operationId: service_plan
      x-api-path-slug: adminapiservicesservice-idservice-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the service plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Set
      - To
      - Default
---