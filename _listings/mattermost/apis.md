---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Commands
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Reference - List autocomplete commands
  x-api-slug: teamsteam-idcommandsautocomplete-get
  description: |-
    List autocomplete commands in the team.
    ##### Permissions
    `view_team` for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-openapi.md
- name: Mattermost API Reference - Create a command
  x-api-slug: commands-post
  description: |-
    Create a command for a team.
    ##### Permissions
    `manage_slash_commands` for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-post-openapi.md
- name: Mattermost API Reference - Update a command
  x-api-slug: commandscommand-id-put
  description: |-
    Update a single command based on command id string and Command struct.
    ##### Permissions
    Must have `manage_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandscommand-id-put-openapi.md
- name: Mattermost API Reference - Delete a command
  x-api-slug: commandscommand-id-delete
  description: |-
    Delete a command based on command id string.
    ##### Permissions
    Must have `manage_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandscommand-id-delete-openapi.md
- name: Mattermost API Reference - Execute a command
  x-api-slug: commandsexecute-post
  description: |-
    Execute a command on a team.
    ##### Permissions
    Must have `use_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandsexecute-post-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - Create a command
  x-api-slug: commands-post
  description: |-
    Create a command for a team.
    ##### Permissions
    `manage_slash_commands` for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-post-openapi.md
- name: Mattermost API Reference - Update a command
  x-api-slug: commandscommand-id-put
  description: |-
    Update a single command based on command id string and Command struct.
    ##### Permissions
    Must have `manage_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandscommand-id-put-openapi.md
- name: Mattermost API Reference - Delete a command
  x-api-slug: commandscommand-id-delete
  description: |-
    Delete a command based on command id string.
    ##### Permissions
    Must have `manage_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandscommand-id-delete-openapi.md
- name: Mattermost API Reference - Execute a command
  x-api-slug: commandsexecute-post
  description: |-
    Execute a command on a team.
    ##### Permissions
    Must have `use_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandsexecute-post-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - Execute a command
  x-api-slug: commandsexecute-post
  description: |-
    Execute a command on a team.
    ##### Permissions
    Must have `use_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandsexecute-post-openapi.md
- name: Mattermost API Reference - Delete a command
  x-api-slug: commandscommand-id-delete
  description: |-
    Delete a command based on command id string.
    ##### Permissions
    Must have `manage_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandscommand-id-delete-openapi.md
- name: Mattermost API Reference - Update a command
  x-api-slug: commandscommand-id-put
  description: |-
    Update a single command based on command id string and Command struct.
    ##### Permissions
    Must have `manage_slash_commands` permission for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commandscommand-id-put-openapi.md
- name: Mattermost API Reference - Create a command
  x-api-slug: commands-post
  description: |-
    Create a command for a team.
    ##### Permissions
    `manage_slash_commands` for the team the command is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-post-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/commands/master/_listings/mattermost/commands-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://matrix.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mattermost.stack.network
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---