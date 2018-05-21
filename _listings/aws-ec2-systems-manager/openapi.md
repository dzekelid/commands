---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListCommands:
    get:
      summary: List Commands
      description: Lists the commands requested by users of the AWS account.
      operationId: listCommands
      x-api-path-slug: actionlistcommands-get
      parameters:
      - in: query
        name: CommandId
        description: (Optional) If provided, lists only the specified command
        type: string
      - in: query
        name: Filters
        description: (Optional) One or more filters
        type: string
      - in: query
        name: InstanceId
        description: (Optional) Lists commands issued against this instance ID
        type: string
      - in: query
        name: MaxResults
        description: (Optional) The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: (Optional) The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Commands
---