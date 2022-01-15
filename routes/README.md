---
description: >-
    List of all routes and their description
---

### GET /player/{id}

Returns player with given id (id is uuid (with or without dashes) or player nickname)

### GET /player/{id}/location

Returns location of player with given id

### POST /player/{selector}/send

Sends message to players by given selector

### PUT /player/{selector}/ban

Bans players by given selector. Reason of ban describes in body

### DELETE /player/{selector}/kick

Kicks players by given selector. Reason of kick describes in body

### DELETE /player/{selector}/kill

Kills players by given selector

### GET /player/{id}/inventory

Returns inventory object of player with given id

### GET /player/{id}/inventory/{item}

Returns item from inventory of player with given id

### POST /player/{id}/link

Sends request to player to link with him. Link request describes in body

### GET /players/list

Returns array of uuids of all online players

### GET /offline/{id}

Returns offline player with given id

### PUT /offline/{selector}/ban

Bans offline players by given selector. Reason of ban describes in body

### GET /bot/{selector}/linked

Returns bot links by given selector

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