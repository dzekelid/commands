---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
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
---