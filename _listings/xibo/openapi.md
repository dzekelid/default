swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /display/defaultlayout/{displayId}:
    post:
      summary: Set Default Layout
      description: Sent the default Layout on this Display
      operationId: displayDefaultLayout
      x-api-path-slug: displaydefaultlayoutdisplayid-post
      parameters:
      - in: path
        name: displayId
        description: The Display ID
      - in: formData
        name: layoutId
        description: The Layout ID
      responses:
        200:
          description: OK
      tags:
      - Set
      - Default
      - Layout