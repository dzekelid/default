---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Describe Engine Default Parameters
  version: 1.0.0
  description: Returns the default engine and system parameter information for the
    specified database engine.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEngineDefaultClusterParameters:
    get:
      summary: Describe Engine Default Cluster Parameters
      description: Returns the default engine and system parameter information for
        the cluster database engine.
      operationId: describeenginedefaultclusterparameters
      x-api-path-slug: actiondescribeenginedefaultclusterparameters-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of the DB cluster parameter group family to return engine
          parameter information for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      DescribeEngineDefaultClusterParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Cluster Parameters
  /?Action=DescribeEngineDefaultParameters:
    get:
      summary: Describe Engine Default Parameters
      description: Returns the default engine and system parameter information for
        the specified database engine.
      operationId: describeenginedefaultparameters
      x-api-path-slug: actiondescribeenginedefaultparameters-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of the DB parameter group family
        type: string
      - in: query
        name: Filters.Filter.N
        description: Not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeEngineDefaultParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Parameters
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