---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API List autocomplete commands
  description: |-
    List autocomplete commands in the team.
    ##### Permissions
    `view_team` for the team.
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