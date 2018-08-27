swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
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