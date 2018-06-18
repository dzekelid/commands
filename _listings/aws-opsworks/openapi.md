---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCommands:
    get:
      summary: Describe Commands
      description: Describes the results of specified commands.
      operationId: describeCommands
      x-api-path-slug: actiondescribecommands-get
      parameters:
      - in: query
        name: CommandIds
        description: An array of command IDs
        type: string
      - in: query
        name: DeploymentId
        description: The deployment ID
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Commands
---