---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API List commands for a team
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
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
  /commands:
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