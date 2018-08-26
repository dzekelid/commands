---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/services/mattermost-slash-commands:
    put:
      summary: Put Projects Services Mattermost Slash Commands
      description: Set mattermost-slash-commands service for project
      operationId: putV3ProjectsIdServicesMattermostSlashCommands
      x-api-path-slug: v3projectsidservicesmattermostslashcommands-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: token
        description: The Mattermost token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Mattermost
      - Slash
      - Commands
  /v3/projects/{id}/services/slack-slash-commands:
    put:
      summary: Put Projects Services Slack Slash Commands
      description: Set slack-slash-commands service for project
      operationId: putV3ProjectsIdServicesSlackSlashCommands
      x-api-path-slug: v3projectsidservicesslackslashcommands-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: token
        description: The Slack token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Slack
      - Slash
      - Commands
  /v3/projects/{id}/services/mattermost_slash_commands/trigger:
    post:
      summary: Post Projects Services Mattermost Slash Commands Trigger
      description: Post projects services mattermost slash commands trigger.
      operationId: postV3ProjectsIdServicesMattermostSlashCommandsTrigger
      x-api-path-slug: v3projectsidservicesmattermost-slash-commandstrigger-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: token
        description: The Mattermost token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Mattermost
      - Slash
      - Commands
      - Trigger
  /v3/projects/{id}/services/slack_slash_commands/trigger:
    post:
      summary: Post Projects Services Slack Slash Commands Trigger
      description: Post projects services slack slash commands trigger.
      operationId: postV3ProjectsIdServicesSlackSlashCommandsTrigger
      x-api-path-slug: v3projectsidservicesslack-slash-commandstrigger-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: token
        description: The Slack token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Slack
      - Slash
      - Commands
      - Trigger
---