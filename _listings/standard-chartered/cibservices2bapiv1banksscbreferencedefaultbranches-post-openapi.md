---
swagger: "2.0"
x-collection-name: Standard Chartered
x-complete: 0
info:
  title: Standard Chartered Bank Code Inquiry
  description: The ???GetBankCode??? API returns list of Bank Codes for the specified
    combination of ???Country???, ???City??? and ???Bank??? combination. The data
    will contain the ???Bank Code(s)??? as well as the address for the Bank & Branch.
  termsOfService: https://www.sc.com/terms-and-conditions
  contact:
    name: Steve Spicer
    url: https://www.sc.com
    email: steven.spicer@sc.com
  version: 1.0.0
host: developer.sc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cib/service/s2b/api/v1/banks/scb/reference/default/branches:
    post:
      summary: Bank Code Inquiry
      description: The ???GetBankCode??? API returns list of Bank Codes for the specified
        combination of ???Country???, ???City??? and ???Bank??? combination. The data
        will contain the ???Bank Code(s)??? as well as the address for the Bank &
        Branch.
      operationId: postCibServiceS2bApiV1BanksScbReferenceDefaultBranches
      x-api-path-slug: cibservices2bapiv1banksscbreferencedefaultbranches-post
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Banking
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Banks
      - Scb
      - Reference
      - Default
      - Branches
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