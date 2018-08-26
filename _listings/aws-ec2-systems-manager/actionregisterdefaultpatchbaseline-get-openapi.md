---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Register Default Patch Baseline
  version: 1.0.0
  description: Defines the default patch baseline.
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