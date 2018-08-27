---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Command Add
  description: Add a Command
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
  /command:
    get:
      summary: Command Search
      description: Search this users Commands
      operationId: commandSearch
      x-api-path-slug: command-get
      parameters:
      - in: formData
        name: code
        description: Filter by Command Code
      - in: formData
        name: command
        description: Filter by Command Name
      - in: formData
        name: commandId
        description: Filter by Command Id
      responses:
        200:
          description: OK
      tags:
      - Command
      - Search
    post:
      summary: Command Add
      description: Add a Command
      operationId: commandAdd
      x-api-path-slug: command-post
      parameters:
      - in: formData
        name: code
        description: A unique code for this command
      - in: formData
        name: command
        description: The Command Name
      - in: formData
        name: description
        description: A description for the command
      responses:
        200:
          description: OK
      tags:
      - Command
  /command/{commandId}:
    put:
      summary: Edit Command
      description: Edit the provided command
      operationId: commandEdit
      x-api-path-slug: commandcommandid-put
      parameters:
      - in: formData
        name: command
        description: The Command Name
      - in: path
        name: commandId
        description: The Command Id to Edit
      - in: formData
        name: description
        description: A description for the command
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Command
    delete:
      summary: Delete Command
      description: Delete the provided command
      operationId: commandDelete
      x-api-path-slug: commandcommandid-delete
      parameters:
      - in: path
        name: commandId
        description: The Command Id to Delete
      responses:
        200:
          description: OK
      tags:
      - Command
  /displaygroup/{displayGroupId}/action/command:
    post:
      summary: Send Command
      description: Send a predefined command to this Group of Displays
      operationId: displayGroupActionCommand
      x-api-path-slug: displaygroupdisplaygroupidactioncommand-post
      parameters:
      - in: formData
        name: commandId
        description: The Command Id
      - in: path
        name: displayGroupId
        description: The display group id
      responses:
        200:
          description: OK
      tags:
      - Send
      - Command
  /playlist/widget/shellCommand/{playlistId}:
    post:
      summary: Add a Shell Command Widget
      description: Add a new Shell Command Widget to the specified playlist
      operationId: WidgetShellCommandAdd
      x-api-path-slug: playlistwidgetshellcommandplaylistid-post
      parameters:
      - in: formData
        name: commandCode
        description: Enter a reference code for exiting command in CMS
      - in: formData
        name: duration
        description: The Widget Duration
      - in: formData
        name: launchThroughCmd
        description: flag (0,1) Windows only, Should the player launch this command
          through the windows command line (cmd
      - in: formData
        name: linuxCommand
        description: Enter a Android / Linux command line compatible command
      - in: formData
        name: name
        description: Optional Widget Name
      - in: path
        name: playlistId
        description: The playlist ID to add a Widget to
      - in: formData
        name: terminateCommand
        description: flag (0,1) Should the player forcefully terminate the command
          after the duration specified, 0 to let the command terminate naturally
      - in: formData
        name: useDuration
        description: (0, 1) Select 1 only if you will provide duration parameter as
          well
      - in: formData
        name: useTaskkill
        description: flag (0,1) Windows only, should the player use taskkill to terminate
          commands
      - in: formData
        name: windowsCommand
        description: Enter a Windows command line compatible command
      responses:
        200:
          description: OK
      tags:
      - Shell
      - Command
      - Widget
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