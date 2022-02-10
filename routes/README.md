---
description: >-
    List of all routes and their description
---

### GET /player/{id}

Returns [player](../objects/entity/living/player.md) with given [id](../objects/entity/living/player.md#id)

### GET /player/{id}/location

Returns [location](../objects/location.md) of player with given [id](../objects/entity/living/player.md#id)

### POST /player/{selector}/send

Sends message to [players](../objects/entity/living/player.md) by given [selector](../objects/entity/living/player.md#selector)

### PUT /player/{selector}/ban

Bans [players](../objects/entity/living/player.md) by given [selector](../objects/entity/living/player.md#selector). Reason of ban describes in body

### DELETE /player/{selector}/kick

Kicks [players](../objects/entity/living/player.md) by given [selector](../objects/entity/living/player.md#selector). Reason of kick describes in body

### DELETE /player/{selector}/kill

Kills [players](../objects/entity/living/player.md) by given [selector](../objects/entity/living/player.md#selector)

### GET /player/{id}/inventory

Returns [inventory object](../objects/inventory/README.md) of [player](../objects/entity/living/player.md) with given [id](../objects/entity/living/player.md#id)

### GET /player/{id}/inventory/{item}

Returns [item](../objects/inventory/item_stack/README.md) from [inventory](../objects/inventory/README.md) of [player](../objects/entity/living/player.md) with given [id](../objects/entity/living/player.md#id)

### POST /player/{id}/link

Sends request to [player](../objects/entity/living/player.md) to link with him. Link request describes in body

### GET /players/list

Returns array of uuids of all online [players](../objects/entity/living/player.md)

### GET /offline/{id}

Returns [offline player](../objects/offline_player.md) with given [id](../objects/offline_player.md#id)

### PUT /offline/{selector}/ban

Bans [offline players](../objects/offline_player.md) by given [selector](../objects/offline_player.md#selector). Reason of ban describes in body

### GET /bot/{selector}/linked

Returns [bot](../objects/bot.md) links by given [selector](../objects/bot.md#selector)

### GET /bot/{selector}/permission/{permission}

Returns [bot](../objects/bot.md) global permission

### GET /bot/{selector}/permission/{permission}/{target}

Returns [bot](../objects/bot.md) target permission

### POST /command

Creates [bot](../objects/bot.md) command. Command describes in body

### DELETE /command/{name}

Deletes [bot](../objects/bot.md) command with given path (Spaces replaced by '_')

### GET /world/{id}

Returns [world](../objects/world.md) with given [id](../objects/world.md#id)

### GET /world/{id}/block/{x}/{y}/{z}

Returns [block](../objects/block.md) with given coordinates from [world](../objects/world.md) with given [id](../objects/world.md#id)

### GET /world/{id}/block/{x}/{y}/{z}/data

Returns block data with given coordinates from [world](../objects/world.md) with given id

### GET /world/{id}/block/{x}/{y}/{z}/data/inventory

Returns [inventory](../objects/inventory/README.md) object of [block](../objects/block.md) with given coordinates from [world](../objects/world.md) with given id

### GET /world/{id}/block/{x}/{y}/{z}/data/inventory/{item}

Returns [item](../objects/inventory/item_stack/README.md) from [inventory](../objects/inventory/README.md) of [block](../objects/block.md) with given coordinates from [world](../objects/world.md) with given id

### PUT /world/{id}/block/{x}/{y}/{z}/data/{name}

Sets field with given name of block data with given coordinates from [world](../objects/world.md) with given id

### GET /player/{id}/ender

Returns ender chest [inventory](../objects/inventory/README.md) of [player](../objects/entity/living/player.md) with given [id](../objects/entity/living/player.md#id)

### GET /player/{id}/ender/{item}

Returns [item](../objects/inventory/item_stack/README.md) from ender chest of [player](../objects/entity/living/player.md) with given [id](../objects/entity/living/player.md#id)

### GET /entity/{id}

Returns entity with given id

### PUT /entity/{id}/capture

Captures entity with given id

### PUT /player/{selector}/inventory/open

Opens [inventory](../objects/inventory/README.md) for player by given selector. Inventory is described in body

### DELETE /player/{selector}/inventory/close

Closes [inventory](../objects/inventory/README.md) for player by given selector