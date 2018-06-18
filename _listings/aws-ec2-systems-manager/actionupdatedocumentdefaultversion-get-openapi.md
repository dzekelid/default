---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Update Document Default Version
  version: 1.0.0
  description: Set the default version of a document.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDefaultPatchBaseline:
    get:
      summary: Get Default Patch Baseline
      description: Retrieves the default patch baseline.
      operationId: getDefaultPatchBaseline
      x-api-path-slug: actiongetdefaultpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the default patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default
      - Baseline
  /?Action=RegisterDefaultPatchBaseline:
    get:
      summary: Register Default Patch Baseline
      description: Defines the default patch baseline.
      operationId: registerDefaultPatchBaseline
      x-api-path-slug: actionregisterdefaultpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline that should be the default patch
          baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Default
      - Baseline
  /?Action=UpdateDocumentDefaultVersion:
    get:
      summary: Update Document Default Version
      description: Set the default version of a document.
      operationId: updateDocumentDefaultVersion
      x-api-path-slug: actionupdatedocumentdefaultversion-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The version of a custom document that you want to set as the
          default version
        type: string
      - in: query
        name: Name
        description: The name of a custom document that you want to set as the default
          version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
      - Default
      - Version
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