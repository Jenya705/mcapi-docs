---
description: >-
    Fully commented config.yml file
---

```yml
__globals__:
  # Message used in linking message (access to command)
  contentMinecraftCommandListElementRepresentation: '&7- &eAccess to %command%'
  # Message used in linking message (not optional permission)
  contentRequiredListElementRepresentation: '&7- &e%permission%'
  # Message used in linking message (optional permission)
  contentOptionalListElementRepresentation: '&7- &e%permission% &7- '
  # List delimiter (\n&r)
  listsDelimiter: |
    &r
global: {
  # Is bot name need to be unique
  botNameUnique: true
}
worker: {
  # How many threads mcapi worker will use (not positive value if all async functions need to be sync)
  threads: 4
}
database:
  # Database user password
  password: '1'
  # Database name
  database: minecraft
  cache: {
    # Links cache size
    botLinksCacheSize: 500,
    # Target links cache size
    targetLinksCacheSize: 500,
    # Bots cache size
    botCacheSize: 500,
    # Permissions cache size
    permissionCacheSize: 500
  }
  # Database host
  host: localhost:3306
  # Database type
  type: sqlite
  # Database user name
  user: root
# Bot commands module configuration
customCommands:
  # Bot command containers configuration (shared for every bot command)
  container:
    # Will print if player is not permitted to use this command
    notPermittedMessage: __inherit__notPermitted
    # Help layout
    helpLayout: |-
      &eHelp:
      %list%
    # Help list delimiter
    helpListDelimiter: __inherit__listsDelimiter
    # Help command element
    helpElement: '&7- <click:suggest_command:%command%>&e%name%</click>'
  # Max command options
  maxCommandOptions: 10
  # Command name pattern
  commandNamePattern: '[a-zA-Z0-9_]*'
  # Stringful parser configuration
  command:
    # Will print to player if not enough arguments
    notEnoughArguments: __inherit__notEnoughArguments
    # Will print to player if argument parsing failed (for example: hi is not integer, it will print the error)
    argumentParseFailed: __inherit__argumentParseFailed
# Linking module configuration
linking:
  # Disable optional permission text
  contentOptionalToggleFalse: '&c&nDisable'
  # Optional permission text
  contentOptionalElement: __inherit__contentOptionalListElementRepresentation
  # Linked success text
  enabledEnd: '&aSuccess!'
  # Decline link button text
  declineButton: '&cDecline'
  # Required permission text
  contentRequiredElement: __inherit__contentRequiredListElementRepresentation
  # Linking title
  title: '&eLinking with %bot_name%'
  # Link message components
  linkMessageComponents: [
    title,
    newline,
    content,
    newline,
    accept,
    ' ',
    decline]
  # Linked declined text
  disabledEnd: '&cDeclined!'
  # Content layout (form name: 'content')
  contentLayout: |-
    &e%bot_name% want this permissions
    %list%
  # Content layout delimiter
  contentDelimiter: __inherit__listsDelimiter
  # Minecraft command representation text
  contentMinecraftCommandElement: __inherit__contentMinecraftCommandListElementRepresentation
  # Minecraft command list layout
  contentMinecraftCommandLayout: |2-

    &eAnd give access to commands
    %list%
  # Enable optional permission text
  contentOptionalToggleTrue: '&a&nEnable'
  # Accept link button text
  acceptButton: '&aAccept'
# Bot module configuration
bot: {
  # Name pattern
  namePattern: '[a-zA-Z0-9_]*'
}
# Web module configuration
web: {
  # Http server port
  port: 8080
}
# Optional debug (if set to true some debug information will appear in console)
debug: false
```