---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Describe Engine Default Parameters
  version: 1.0.0
  description: |-
    Returns the default engine and
                system parameter information for the specified cache engine.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEngineDefaultParameters:
    get:
      summary: Describe Engine Default Parameters
      description: |-
        Returns the default engine and
                    system parameter information for the specified cache engine.
      operationId: describeEngineDefaultParameters
      x-api-path-slug: actiondescribeenginedefaultparameters-get
      parameters:
      - in: query
        name: CacheParameterGroupFamily
        description: The name of the cache parameter group family
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Engine Default Parameters
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