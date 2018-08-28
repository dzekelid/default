swagger: "2.0"
x-collection-name: Pingdom
x-complete: 1
info:
  title: Traceroute API
  description: the-traceroute-api-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: api.pingdom.com
basePath: /
paths:
  ? |2-

        /api/{version}/summary.outage/{checkid}
  : ? |2-

          get
    : summary: Get List of Outages
      description: Get a list of status changes for a specified check and time period.
        If order is speficied to descending, the list is ordered by newest first.
        (Default is ordered by oldest first.)
      operationId: get-list-of-outages
      x-api-path-slug: apiversionsummary-outagecheckid-get
      parameters:
      - in: query
        name: from
        description: Start time of period
        type: <td>integer</td>
      - in: query
        name: order
        description: Sorting order of outages
        type: <td>string (asc,desc)</td>
      - in: query
        name: to
        description: End time of period
        type: <td>integer</td>
      responses:
        "":
          description: ""
        400:
          description: Bad input parameter
        401:
          description: Bad or expired token
        403:
          description: Bad OAuth request (wrong consumer key, bad nonce, expired timestamp
        404:
          description: File or folder not found at the specified path
        405:
          description: Request method not expected (generally should be GET or POST)
        429:
          description: Your app is making too many requests and is being rate limited
        503:
          description: If the response includes the Retry-After header, this means
            your OAuth 1
        507:
          description: User is over Dropbox storage quota
        5xx:
          description: Server error
      tags:
      - Summary