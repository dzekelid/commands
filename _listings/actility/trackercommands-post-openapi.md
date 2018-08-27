---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Location API Tracker command sending
  description: Sends a downlink command to a supported Abeeway tracker.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /location/v110
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trackerCommands:
    post:
      summary: Tracker command sending
      description: Sends a downlink command to a supported Abeeway tracker.
      operationId: sends-a-downlink-command-to-a-supported-abeeway-tracker
      x-api-path-slug: trackercommands-post
      parameters:
      - in: body
        name: trackerCommand
        description: Contents of the tracker command
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tracker
      - Command
      - Sending
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