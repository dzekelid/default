---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get all project roles
  description: |-
    Gets a list of all project roles, complete with project role details and default actors.

    ### About project roles

    [Project roles](https://confluence.atlassian.com/x/3odKLg) are a flexible way to to associate users and groups with projects. In Jira Cloud, the list of project roles is shared globally with all projects, but each project can have a different set of actors associated with it (unlike groups, which have the same membership throughout all Jira applications).

    Project roles can be used in [permission schemes](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-permissionscheme-get), [email notification schemes](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-notificationscheme-get), [issue security levels](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-issuesecurityschemes-get), [comment visibility](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-comment-list-post), and workflow conditions.

    #### Members and actors

    In the Jira REST API, a member of a project role is called an _actor_. An _actor_ is a group or user associated with a project role.

    Actors may be set as [default members](https://confluence.atlassian.com/x/3odKLg#Managingprojectroles-Specifying'defaultmembers'foraprojectrole) of the project role or set at the project level:

    *   Default actors: Users and groups that are assigned to the project role for all newly created projects. The default actors can be removed at the project level later if desired.
    *   Actors: Users and groups that are associated with a project role for a particular project, which may differ from the default actors. This allows you to assign a particular user to different roles in different projects.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
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
  /api/2/user/columns:
    get:
      summary: Get user default columns
      description: |-
        Returns the default [issue table columns](https://confluence.atlassian.com/x/XYdKLg) for the user. If a username is not passed in the request, the calling user's details are returned. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To get the column details for any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLgl).
        *   To get the calling user's column details: None
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.getUserDefaultColumns_get
      x-api-path-slug: api2usercolumns-get
      parameters:
      - in: query
        name: accountId
        description: the account ID
      - in: header
        name: force-account-id
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - User
      - Default
      - Columns
    put:
      summary: Set user default columns
      description: |-
        Sets the default [issue table columns](https://confluence.atlassian.com/x/XYdKLg) for the user. If a username is not passed, the calling user's default columns are set. If no column details are sent, then all default columns are removed. The parameters for this resource are expressed as HTML form data. For example, in curl: `curl -X PUT -d username= -d columns=summary -d columns=description ` **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To set the columns on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To set the calling user's columns: None
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.setUserColumns_put
      x-api-path-slug: api2usercolumns-put
      parameters:
      - in: query
        name: accountId
        description: the account ID
      - in: header
        name: force-account-id
      responses:
        200:
          description: OK
      tags:
      - Set
      - User
      - Default
      - Columns
    delete:
      summary: Reset user default columns
      description: |-
        Resets the default [issue table columns](https://confluence.atlassian.com/x/XYdKLg) for the user to the system default. If a username is not passed, the calling user's default columns are reset. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To set the columns on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To set the calling user's columns: None
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.resetUserColumns_delete
      x-api-path-slug: api2usercolumns-delete
      parameters:
      - in: query
        name: accountId
        description: the account ID
      - in: header
        name: force-account-id
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - Reset
      - User
      - Default
      - Columns
  /api/2/workflowscheme/{id}/default:
    get:
      summary: Get default workflow
      description: Return the default workflow from the passed workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getDefaultWorkflow_get
      x-api-path-slug: api2workflowschemeiddefault-get
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      - in: query
        name: returnDraftIfExists
        description: when true indicates that a schemes draft, if it exists, should
          be queried instead of the scheme itself
      responses:
        200:
          description: OK
      tags:
      - Default
      - Workflow
    put:
      summary: Update default workflow
      description: |-
        Set the default workflow for the passed workflow scheme.

        The passed representation can have its updateDraftIfNeeded flag set to true to indicate that the draft should be created/updated when the actual scheme cannot be edited.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.updateDefaultWorkflow_put
      x-api-path-slug: api2workflowschemeiddefault-put
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      responses:
        200:
          description: OK
      tags:
      - Default
      - Workflow
    delete:
      summary: Delete default workflow
      description: Remove the default workflow from the passed workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteDefaultWorkflow_delete
      x-api-path-slug: api2workflowschemeiddefault-delete
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      - in: query
        name: updateDraftIfNeeded
        description: when true will create and return a draft when the workflow scheme
          cannot be edited (e
      responses:
        200:
          description: OK
      tags:
      - Default
      - Workflow
  /api/2/workflowscheme/{id}/draft/default:
    get:
      summary: Get draft default workflow
      description: Return the default workflow from the passed draft workflow scheme
        to the caller.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getDraftDefaultWorkflow_get
      x-api-path-slug: api2workflowschemeiddraftdefault-get
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Default
      - Workflow
    put:
      summary: Update draft default workflow
      description: Set the default workflow for the passed draft workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.updateDraftDefaultWorkflow_pu
      x-api-path-slug: api2workflowschemeiddraftdefault-put
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Default
      - Workflow
    delete:
      summary: Delete draft default workflow
      description: Remove the default workflow from the passed draft workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteDraftDefaultWorkflow_de
      x-api-path-slug: api2workflowschemeiddraftdefault-delete
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Default
      - Workflow
  /api/2/role:
    get:
      summary: Get all project roles
      description: |-
        Gets a list of all project roles, complete with project role details and default actors.

        ### About project roles

        [Project roles](https://confluence.atlassian.com/x/3odKLg) are a flexible way to to associate users and groups with projects. In Jira Cloud, the list of project roles is shared globally with all projects, but each project can have a different set of actors associated with it (unlike groups, which have the same membership throughout all Jira applications).

        Project roles can be used in [permission schemes](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-permissionscheme-get), [email notification schemes](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-notificationscheme-get), [issue security levels](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-issuesecurityschemes-get), [comment visibility](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-comment-list-post), and workflow conditions.

        #### Members and actors

        In the Jira REST API, a member of a project role is called an _actor_. An _actor_ is a group or user associated with a project role.

        Actors may be set as [default members](https://confluence.atlassian.com/x/3odKLg#Managingprojectroles-Specifying'defaultmembers'foraprojectrole) of the project role or set at the project level:

        *   Default actors: Users and groups that are assigned to the project role for all newly created projects. The default actors can be removed at the project level later if desired.
        *   Actors: Users and groups that are associated with a project role for a particular project, which may differ from the default actors. This allows you to assign a particular user to different roles in different projects.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.getAllProjectRoles_get
      x-api-path-slug: api2role-get
      responses:
        200:
          description: OK
      tags:
      - Project
      - Roles
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