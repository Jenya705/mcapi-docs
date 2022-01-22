---
description: >-
    Description of living entity rest object
---

Living entity inherits Entity, so all entity properties will be moved to living entity

## Fields
ai: Optional Boolean - true if entity has ai otherwise empty
health: Optional Float - health of the entity. Empty if health equals to 20

## Example
```json
{
  "type": "minecraft:pig",
  "location": {
    "world": "minecraft:overworld",
    "x": -1.06,
    "y": -60,
    "z": -38.61
  },
  "health": 10
}
```