---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify assigning a new default address to a customer
  description: Assigning a new default address to a customer.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/customers/3989659651/addresses/5436816654/default.json:
    put:
      summary: assigning a new default address to a customer
      description: Assigning a new default address to a customer.
      operationId: putAdminCustomers3989659651Addresses5436816654Default.json
      x-api-path-slug: admincustomers3989659651addresses5436816654default-json-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Assigning
      - New
      - Default
      - Address
      - To
      - Customer
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