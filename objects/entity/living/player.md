---
description: >-
    Description of player rest object
---

Player inherits Living entity, so all living entity properties will be moved to player

## Abilities

### Fields

invulnerable: Optional Boolean - true if the player is invulnerable otherwise empty

mayFly: Optional Boolean - true if the player may fly otherwise empty

instabuild: Optional Boolean - true if the player may instabuild otherwise empty

walkSpeed: Optional Float - the player walk speed. Empty if walkSpeed is 0.1

mayBuild: Optional Boolean - false if the player may not build otherwise empty

flying: Optional Boolean - true if the player may fly otherwise empty

flySpeed: Optional Float - the player flySpeed. Empty is flySpeed is 0.05

## ID

id of player is uuid or player nickname

## Selector

selector of player:
* @a - all online players
* @r - random online player
* @l - linked online players
* default: player by given [id](#id)

## Fields
gamemode: Enum - current gamemode of the player (SURVIVAL, CREATIVE, ADVENTURE, SPECTATOR)

abilities: Abilities - current abilities of the player

## Example
```json
{
  "name": "Jenya705",
  "uuid": "ca78e928-484b-36ff-bc1e-ade3e86597df",
  "type": "minecraft:player",
  "location": {
    "world": "minecraft:overworld",
    "x": -0.6950000000000001,
    "y": -60,
    "z": -37.9854
  },
  "gameMode": "CREATIVE",
  "abilities": {
    "mayFly": true,
    "instabuild": true
  }
}
```