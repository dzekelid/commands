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
  /?Action=CancelCommand:
    get:
      summary: Cancel Command
      description: Attempts to cancel the command specified by the Command ID.
      operationId: cancelCommand
      x-api-path-slug: actioncancelcommand-get
      parameters:
      - in: query
        name: CommandId
        description: The ID of the command you want to cancel
        type: string
      - in: query
        name: InstanceIds
        description: (Optional) A list of instance IDs on which you want to cancel
          the command
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Command
  /?Action=GetCommandInvocation:
    get:
      summary: Get Command Invocation
      description: Returns detailed information about command execution for an invocation
        or plugin.
      operationId: getCommandInvocation
      x-api-path-slug: actiongetcommandinvocation-get
      parameters:
      - in: query
        name: CommandId
        description: (Required) The parent command ID of the invocation plugin
        type: string
      - in: query
        name: InstanceId
        description: (Required) The ID of the managed instance targeted by the command
        type: string
      - in: query
        name: PluginName
        description: (Optional) The name of the plugin for which you want detailed
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Command
      - Invocation
  /?Action=ListCommandInvocations:
    get:
      summary: List Command Invocations
      description: An invocation is copy of a command sent to a specific instance.
      operationId: listCommandInvocations
      x-api-path-slug: actionlistcommandinvocations-get
      parameters:
      - in: query
        name: CommandId
        description: (Optional) The invocations for a specific command ID
        type: string
      - in: query
        name: Details
        description: (Optional) If set this returns the response of the command executions
          and any command   output
        type: string
      - in: query
        name: Filters
        description: (Optional) One or more filters
        type: string
      - in: query
        name: InstanceId
        description: (Optional) The command execution details for a specific instance
          ID
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
      - Command
      - Invocations
  /?Action=SendCommand:
    get:
      summary: Send Command
      description: Executes commands on one or more remote instances.
      operationId: sendCommand
      x-api-path-slug: actionsendcommand-get
      parameters:
      - in: query
        name: Comment
        description: User-specified information about the command, such as a brief
          description of what the   command should do
        type: string
      - in: query
        name: DocumentHash
        description: The Sha256 or Sha1 hash created by the system when the document
          was created
        type: string
      - in: query
        name: DocumentHashType
        description: Sha256 or Sha1
        type: string
      - in: query
        name: DocumentName
        description: Required
        type: string
      - in: query
        name: InstanceIds
        description: Required
        type: string
      - in: query
        name: MaxConcurrency
        description: (Optional) The maximum number of instances that are allowed to
          execute the command at the   same time
        type: string
      - in: query
        name: MaxErrors
        description: The maximum number of errors allowed without the command failing
        type: string
      - in: query
        name: NotificationConfig
        description: Configurations for sending notifications
        type: string
      - in: query
        name: OutputS3BucketName
        description: The name of the S3 bucket where command execution responses should
          be stored
        type: string
      - in: query
        name: OutputS3KeyPrefix
        description: The directory structure within the S3 bucket where the responses
          should be   stored
        type: string
      - in: query
        name: OutputS3Region
        description: (Optional) The region where the Amazon Simple Storage Service
          (Amazon S3) output bucket is located
        type: string
      - in: query
        name: Parameters
        description: The required and optional parameters specified in the SSM document
          being   executed
        type: string
      - in: query
        name: ServiceRoleArn
        description: The IAM role that Systems Manager uses to send notifications
        type: string
      - in: query
        name: Targets
        description: (Optional) An array of search criteria that targets instances
          using a    Key;Value combination that you specify
        type: string
      - in: query
        name: TimeoutSeconds
        description: If this time is reached and the command has not already started
          executing, it will not   execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - Send
      - Command
  /?Action=CreateActivation:
    get:
      summary: Create Activation
      description: |-
        Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage
           these resources using Run Command.
      operationId: createActivation
      x-api-path-slug: actioncreateactivation-get
      parameters:
      - in: query
        name: DefaultInstanceName
        description: The name of the registered, managed instance as it will appear
          in the Amazon EC2 console or   when you use the AWS command line tools to
          list EC2 resources
        type: string
      - in: query
        name: Description
        description: A user-defined description of the resource that you want to register
          with Amazon EC2
        type: string
      - in: query
        name: ExpirationDate
        description: The date by which this activation request should expire
        type: string
      - in: query
        name: IamRole
        description: The Amazon Identity and Access Management (IAM) role that you
          want to assign to the   managed instance
        type: string
      - in: query
        name: RegistrationLimit
        description: Specify the maximum number of managed instances you want to register
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activation