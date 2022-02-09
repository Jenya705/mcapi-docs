---
description: >-
    Description of entity rest object
---

## ID

Entity id is it uuid

## Fields

type: Enum - type of the entity

location: Optional [Location](../location.md) - location of the entity

customName: Optional Component - custom name of the entity

## Example
```json
{
  "type": "minecraft:armor_stand",
  "location": {
    "world": "minecraft:overworld",
    "x": -2.5,
    "y": -60,
    "z": -22.5
  }
}
```