---
description: >-
    Fully commented commands.yml
---
```yml
__globals__:
  # Bot link element representation
  linkListElementRepresentation: '&7- &e%name% &7- <click:run_command:/mcapi linkMenu
    permission %bot_id%>&9[Permissions]</click> <click:run_command:/mcapi linkMenu
    unlink %bot_id%>&c[Unlink]</click>'
  # Bot subscription element representation
  subscriptionsElementListRepresentation: '&7- &e%name%'
  # Will be printed if player is not permitted to use command
  notPermitted: '&cYou are not permitted to do that'
  # Will be printed if bot name is not unique
  tooManyBots: '&cToo many bots with given name, please provide the token'
  # Will be printed if bot with given name is not exist
  botNotExist: '&cBot with given name is not exist'
  # Will be printed if player is not linked with bot
  notLinkedWithBot: '&cYou are not linked with this bot'
  # Will be printed if player is not exist (e.g: in argument)
  playerNotFound: '&cGiven player is not exist nor you are not player'
  # Gateway connection representation
  gatewaysElementListRepresentation: '&7- &e%name%'
  # Will be printed if not enough arguments provided
  notEnoughArguments: '&cNot enough arguments'
  # Lists delimiter (\n&r)
  listsDelimiter: |
    &r
  # Will be printed if failed to parse some argument
  argumentParseFailed: '&cFailed to parse %argument_id%'
  # Max elements on page
  maxElementsInList: 10
  # Localizaed permission element representation
  localizedPermissionElementListRepresentation: '&7- &e%permission%'
  # Will be printed if some command disabled in configuration
  disabledByAdmin: '&eThis feature disabled by admin'
  # Will be printed if player try to make bot with length more than 64
  botNameTooLong: '&cBot name too long, maximum length 64'
  # Bot element representation
  botListElementRepresentation: '&7- &9%name% &7- <click:suggest_command:%token%>&e%token%</click>'
notPermittedMessage: __inherit__notPermitted
# Help layout
helpLayout: |-
  &eHelp:
  %list%
# Help element
helpElement: '&7- <click:suggest_command:%command%>&e%name%</click>'
helpListDelimiter: __inherit__listsDelimiter
linkmenu:
  unlink: {
    success: '&cUnlinked!'
  }
  permission:
    listElement: __inherit__localizedPermissionElementListRepresentation
    listDelimiter: __inherit__listsDelimiter
    listLayout: |-
      &ePermissions for %name%
      %list%
unlink: {
  notPermittedForOthers: '&cYou can not unlink for others',
  disabledByAdmin: __inherit__disabledByAdmin,
  notLinked: __inherit__notLinkedWithBot,
  success: '&cUnlinked!',
  playerNotFound: __inherit__playerNotFound,
  notEnoughArguments: __inherit__notEnoughArguments,
  argumentParseFailed: __inherit__argumentParseFailed
}
bot:
  create: {
    notPermittedForOthers: '&cYou can not create bots for others',
    success: '&aSuccess! Created bot with token <click:suggest_command:%token%>&e%token%</click>',
    botNameTooLong: __inherit__botNameTooLong,
    playerNotFound: __inherit__playerNotFound,
    botWithNameExist: '&cChoose another name, because this used',
    notEnoughArguments: __inherit__notEnoughArguments,
    argumentParseFailed: __inherit__argumentParseFailed
  }
  permission:
    give: {
      notPermitted: __inherit__notPermitted,
      success: '&aSuccess',
      tooManyBots: __inherit__tooManyBots,
      botNotExist: __inherit__botNotExist,
      notEnoughArguments: __inherit__notEnoughArguments,
      argumentParseFailed: __inherit__argumentParseFailed
    }
    list:
      listElement: '&7- %toggle%%permission_name%'
      listDelimiter: __inherit__listsDelimiter
      tooManyBots: __inherit__tooManyBots
      notPermitted: __inherit__notPermitted
      botNotExist: __inherit__botNotExist
      maxElements: __inherit__maxElementsInList
      notEnoughArguments: __inherit__notEnoughArguments
      permissionDisabled: '&c'
      permissionEnabled: '&a'
      argumentParseFailed: __inherit__argumentParseFailed
      listLayout: |-
        &ePermissions for %bot_name%
        %list%
        &ePage %page%
  list:
    notPermittedForOthers: '&cYou can not see others bots'
    listElement: __inherit__botListElementRepresentation
    listDelimiter: __inherit__listsDelimiter
    maxElements: __inherit__maxElementsInList
    playerNotFound: __inherit__playerNotFound
    notEnoughArguments: __inherit__notEnoughArguments
    argumentParseFailed: __inherit__argumentParseFailed
    listLayout: |-
      &eBots of player %player_name%
      %list%
      &ePage %page%
  delete: {
    confirm: '&c&lWARNING! &eBot will permanently deleted! Add confirm to the command
      to confirm',
    success: '&cBot deleted',
    notPermitted: __inherit__notPermitted,
    notEnoughArguments: __inherit__notEnoughArguments,
    argumentParseFailed: __inherit__argumentParseFailed
  }
links:
  listElement: __inherit__linkListElementRepresentation
  listDelimiter: __inherit__listsDelimiter
  maxElements: __inherit__maxElementsInList
  playerNotFound: __inherit__playerNotFound
  notEnoughArguments: __inherit__notEnoughArguments
  argumentParseFailed: __inherit__argumentParseFailed
  listLayout: |-
    &eLinks of player %player%
    %list%
    &ePage %page%
tunnel:
  connected:
    listElement: __inherit__gatewaysElementListRepresentation
    listDelimiter: __inherit__listsDelimiter
    maxElements: __inherit__maxElementsInList
    notEnoughArguments: __inherit__notEnoughArguments
    argumentParseFailed: __inherit__argumentParseFailed
    listLayout: |-
      &eConnected event tunnels
      %list%
      Page %page%
  subscriptions:
    listElement: __inherit__subscriptionsElementListRepresentation
    listDelimiter: __inherit__listsDelimiter
    notPermitted: __inherit__notPermitted
    maxElements: __inherit__maxElementsInList
    notEnoughArguments: __inherit__notEnoughArguments
    argumentParseFailed: __inherit__argumentParseFailed
    botIsNotConnected: '&cBot is not connected to gateway'
    listLayout: |-
      &eSubscriptions %name%
      %list%
      Page %page%
```