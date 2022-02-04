---
description: >-
    List of all routes and their description
---

### GET /player/{id}

Returns [player](../objects/entity/living/player.md) with given [id](../objects/entity/living/player.md#id)

### GET /player/{id}/location

Returns location of player with given [id](../objects/entity/living/player.md#id)

### POST /player/{selector}/send

Sends message to [players](../objects/entity/living/player.md) by given [selector](../object/entity/living/player.md#selector)

### PUT /player/{selector}/ban

Bans [players](../objects/entity/living/player.md) by given [selector](../object/entity/living/player.md#selector). Reason of ban describes in body

### DELETE /player/{selector}/kick

Kicks [players](../object/entity/living/player.md) by given [selector](../object/entity/living/player.md#selector). Reason of kick describes in body

### DELETE /player/{selector}/kill

Kills [players](../object/entity/living/player.md) by given [selector](../object/entity/living/player.md#selector)

### GET /player/{id}/inventory

Returns inventory object of [player](../object/entity/living/player.md) with given [id](../object/entity/living/player.md#id)

### GET /player/{id}/inventory/{item}

Returns item from inventory of [player](../object/entity/living/player.md) with given [id](../object/entity/living/player.md#id)

### POST /player/{id}/link

Sends request to [player](../object/entity/living/player.md) to link with him. Link request describes in body

### GET /players/list

Returns array of uuids of all online [players](../object/entity/living/player.md)

### GET /offline/{id}

Returns [offline player](../object/offline_player.md) with given [id](../object/offline_player.md#id)

### PUT /offline/{selector}/ban

Bans [offline players](../object/offline_player.md) by given [selector](../object/offline_player.md#selector). Reason of ban describes in body

### GET /bot/{selector}/linked

Returns bot links by given [selector](../object/bot.md#selector)

### GET /bot/{selector}/permission/{permission}

Returns bot global permission

### GET /bot/{selector}/permission/{permission}/{target}

Returns bot target permission

### POST /command

Creates bot command. Command describes in body

### DELETE /command/{name}

Deletes bot command with given path (Spaces replaced by '_')

### GET /world/{id}

Returns world with given id

### GET /world/{id}/block/{x}/{y}/{z}

Returns block with given coordinates from world with given id

### GET /world/{id}/block/{x}/{y}/{z}/data

Returns block data with given coordinates from world with given id

### GET /world/{id}/block/{x}/{y}/{z}/data/inventory

Returns inventory object of block with given coordinates from world with given id

### GET /world/{id}/block/{x}/{y}/{z}/data/inventory/{item}

Returns item from inventory of block with given coordinates from world with given id

### PUT /world/{id}/block/{x}/{y}/{z}/data/{name}

Sets field with given name of block data with given coordinates from world with given id

### GET /player/{id}/ender

Returns ender chest inventory of player with given id

### GET /player/{id}/ender/{item}

Returns item from ender chest of player with given id

### GET /entity/{id}

Returns entity with given id

### PUT /entity/{id}/capture

Captures entity with given id

### PUT /player/{selector}/inventory/open

Opens inventory for player by given selector. Inventory describes in body

### DELETE /player/{selector}/inventory/close

Closes inventory for player by given selector