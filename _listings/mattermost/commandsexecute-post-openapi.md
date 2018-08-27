---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Execute a command
  description: |-
    Execute a command on a team.
    ##### Permissions
    Must have `use_slash_commands` permission for the team the command is in.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{team_id}/commands/autocomplete:
    get:
      summary: List autocomplete commands
      description: |-
        List autocomplete commands in the team.
        ##### Permissions
        `view_team` for the team.
      operationId: list-autocomplete-commands-in-the-team-permissionsview-team-for-the-team
      x-api-path-slug: teamsteam-idcommandsautocomplete-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - List
      - Autocomplete
      - Commands
  /commands:
    post:
      summary: Create a command
      description: |-
        Create a command for a team.
        ##### Permissions
        `manage_slash_commands` for the team the command is in.
      operationId: create-a-command-for-a-team-permissionsmanage-slash-commands-for-the-team-the-command-is-in
      x-api-path-slug: commands-post
      parameters:
      - in: body
        name: body
        description: command to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Command
    get:
      summary: List commands for a team
      description: |-
        List commands for a team.
        ##### Permissions
        `manage_slash_commands` if need list custom commands.
      operationId: list-commands-for-a-team-permissionsmanage-slash-commands-if-need-list-custom-commands
      x-api-path-slug: commands-get
      parameters:
      - in: query
        name: custom_only
        description: To get only the custom commands
      - in: query
        name: team_id
        description: The team id
      responses:
        200:
          description: OK
      tags:
      - List
      - Commandsa
      - Team
  /commands/{command_id}:
    put:
      summary: Update a command
      description: |-
        Update a single command based on command id string and Command struct.
        ##### Permissions
        Must have `manage_slash_commands` permission for the team the command is in.
      operationId: update-a-single-command-based-on-command-id-string-and-command-struct-permissionsmust-have-manage-sl
      x-api-path-slug: commandscommand-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: command_id
        description: ID of the command to update
      responses:
        200:
          description: OK
      tags:
      - Command
    delete:
      summary: Delete a command
      description: |-
        Delete a command based on command id string.
        ##### Permissions
        Must have `manage_slash_commands` permission for the team the command is in.
      operationId: delete-a-command-based-on-command-id-string-permissionsmust-have-manage-slash-commands-permission-fo
      x-api-path-slug: commandscommand-id-delete
      parameters:
      - in: path
        name: command_id
        description: ID of the command to delete
      responses:
        200:
          description: OK
      tags:
      - Command
  /commands/execute:
    post:
      summary: Execute a command
      description: |-
        Execute a command on a team.
        ##### Permissions
        Must have `use_slash_commands` permission for the team the command is in.
      operationId: execute-a-command-on-a-team-permissionsmust-have-use-slash-commands-permission-for-the-team-the-comm
      x-api-path-slug: commandsexecute-post
      parameters:
      - in: body
        name: body
        description: command to be executed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Command
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