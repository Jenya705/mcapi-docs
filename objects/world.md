---
description: >-
    Description of world rest object
---

## ID

World id is key of the world namespace (overworld, the_nether, the_end, etc.)

## Fields
name: String - namespace of the world

dimension: Enum - dimension of the world (OVERWORLD, NETHER, END, CUSTOM)

weather: Enum - weather of the world (CLEAR, RAIN, THUNDER)

## Example
```json
{
  "name": "minecraft:overworld",
  "dimension": "OVERWORLD",
  "weather": "CLEAR"
}
```