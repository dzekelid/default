---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Set issue navigator default columns
  description: Sets the default system columns for issue navigator. Admin permission
    will be required.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/filter/defaultShareScope:
    get:
      summary: Get default share scope
      description: Returns the default sharing settings for new filters and dashboards
        for a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
        Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getDefaultShareScope_get
      x-api-path-slug: api2filterdefaultsharescope-get
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
        200:
          description: OK
      tags:
      - Default
      - Share
      - Scope
    put:
      summary: Set default share scope
      description: Sets the default sharing for new filters and dashboards for a user.
        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
        to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.setDefaultShareScope_put
      x-api-path-slug: api2filterdefaultsharescope-put
      responses:
        200:
          description: OK
      tags:
      - Set
      - Default
      - Share
      - Scope
  /api/2/role/{id}/actors:
    get:
      summary: Get default actors for project role
      description: |-
        Returns the [default actors](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-resolution-get) for the project role.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.getProjectRoleActorsForRole_get
      x-api-path-slug: api2roleidactors-get
      parameters:
      - in: path
        name: id
        description: The ID of the project role
      responses:
        200:
          description: OK
      tags:
      - Default
      - Actorsproject
      - Role
    post:
      summary: Add default actors to project role
      description: |-
        Adds [default actors](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-resolution-get) to the given role. You may add either groups or users, but you cannot add groups and users in the same request.

        Changing a project role's default actors does not affect project role members for projects already created.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.addProjectRoleActorsToRole_post
      x-api-path-slug: api2roleidactors-post
      parameters:
      - in: header
        name: force-account-id
      - in: path
        name: id
        description: The ID of the project role
      responses:
        200:
          description: OK
      tags:
      - Default
      - Actors
      - To
      - Project
      - Role
    delete:
      summary: Delete default actors from project role
      description: |-
        Removes [default actors](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-resolution-get) from the project role. You may remove either a group or user, but you cannot remove a group and a user in the same request.

        Changing a project role's default actors does not affect project role members for projects already created.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.deleteProjectRoleActorsFromRole_delete
      x-api-path-slug: api2roleidactors-delete
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: group
        description: The group name of the group to be removed as a default actor
      - in: path
        name: id
        description: The ID of the project role
      - in: query
        name: user
        description: The user account ID of the user to remove as a default actor
      responses:
        200:
          description: OK
      tags:
      - Default
      - Actors
      - From
      - Project
      - Role
  /api/2/screens/addToDefault/{fieldId}:
    post:
      summary: Add field to default screen
      description: Adds field or custom field to the default tab
      operationId: com.atlassian.jira.rest.v2.issue.ScreensResource.addFieldToDefaultScreen_post
      x-api-path-slug: api2screensaddtodefaultfieldid-post
      parameters:
      - in: path
        name: fieldId
        description: id of field / custom field
      responses:
        200:
          description: OK
      tags:
      - Field
      - To
      - Default
      - Screen
  /api/2/settings/columns:
    get:
      summary: Get issue navigator default columns
      description: Returns the default system columns for issue navigator. Admin permission
        will be required.
      operationId: com.atlassian.jira.rest.v2.admin.SettingsResource.getIssueNavigatorDefaultColumns_get
      x-api-path-slug: api2settingscolumns-get
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Navigator
      - Default
      - Columns
    put:
      summary: Set issue navigator default columns
      description: Sets the default system columns for issue navigator. Admin permission
        will be required.
      operationId: com.atlassian.jira.rest.v2.admin.SettingsResource.setIssueNavigatorDefaultColumns_put
      x-api-path-slug: api2settingscolumns-put
      responses:
        200:
          description: OK
      tags:
      - Set
      - Issue
      - Navigator
      - Default
      - Columns
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