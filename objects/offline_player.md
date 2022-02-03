---
description: >-
    Description of offline player rest object
---

if player online object will be [player](entity/living/player.md)

## Selector

selector of offline player:
* @l - all linked players
* default: offline player by given [id](#id)

## ID

equals to [online player id](entity/living/player.md#id)

## Fields

name: String - offline player name

uuid: UUID - offline player uuid

online: boolean - true if player online otherwise false

## Example
```json
{
  "name": "Jenya705",
  "uuid": "ca78e928-484b-36ff-bc1e-ade3e86597df",
  "online": false
}
```