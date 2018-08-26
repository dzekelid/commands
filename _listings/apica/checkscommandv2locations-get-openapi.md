---
swagger: "2.0"
x-collection-name: Apica
x-complete: 0
info:
  title: Checks Command API Checks Command Locations
  version: 1.0.0
  description: Gets a list of all locations that are available for Command checks
    (version 2).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/checks/command ':
    ' post ':
      summary: Checks Command
      description: Creates a new Command check.
      operationId: -checks-command-
      x-api-path-slug: checkscommand-post
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Command
  '/checks/command-v2 ':
    ' post ':
      summary: Checks Command
      description: Creates a new Command check (version 2).
      operationId: -checks-command-v2-
      x-api-path-slug: checkscommandv2-post
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Command
  '/checks/command-v2/{checkId} ':
    ' put ':
      summary: Checks Command
      description: Updates a command check (version 2).
      operationId: -checks-command-v2-checkid-
      x-api-path-slug: checkscommandv2checkid-put
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Command
  '/checks/command/{checkId} ':
    ' put ':
      summary: Checks Command
      description: Updates a command check.
      operationId: -checks-command-checkid-
      x-api-path-slug: checkscommandcheckid-put
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Command
  '/checks/command/categories ':
    ' get ':
      summary: Checks Command Categories
      description: Gets a list of all command check categories that are available
        for you as customer.
      operationId: -checks-command-categories-
      x-api-path-slug: checkscommandcategories-get
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Command
  '/checks/command-v2/categories ':
    ' get ':
      summary: Checks Command Categories
      description: Gets a list of all command check (version 2) categories that are
        available for you as customer.
      operationId: -checks-command-v2-categories-
      x-api-path-slug: checkscommandv2categories-get
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Command
  '/checks/command/locations ':
    ' get ':
      summary: Checks Command Locations
      description: Gets a list of all locations that are available for Command checks.
      operationId: -checks-command-locations-
      x-api-path-slug: checkscommandlocations-get
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Command
  /checks/command-v2/locations:
    ' get ':
      summary: Checks Command Locations
      description: Gets a list of all locations that are available for Command checks
        (version 2).
      operationId: -checks-command-v2-locationsprotocolprotocol-
      x-api-path-slug: checkscommandv2locations-get
      responses:
        200:
          description: OK
      tags:
      - Checks
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