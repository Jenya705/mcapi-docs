---
description: >-
    Description of all mcapi commands
---

#### /mcapi bot create <bot_name> [player]
creates bot with given bot name for the given player (by default is sender) and send bot token

#### /mcapi bot delete <token> ['confirm']
deletes bot with given token

#### /mcapi bot list [page] [player]
send given players bots

#### /mcapi bot permission list <bot_name> [is_bot_name_token] [page]
send bot permissions with given bot_name (or token if is_bot_name_token true)

#### /mcapi bot permission give <bot_name> <permission> <toggled> [target] [is_bot_name_token] [is_permission_regex]
give bot permission with given name for target (global if not specified).
If is_permission_regex set to true, permission will be regex

#### /mcapi links [page]
send player links

#### /mcapi tunnel connected [page]
send bots connected to the tunnel

#### /mcapi tunnel subscriptions <token> [page]
send bot subscriptions

#### /mcapi unlink <bot_name> [player]
unlink player and given bot