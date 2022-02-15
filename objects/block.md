---
description: >-
    Description of block rest object
---

## ID

UUID of the block is UUID with mostSigBits = (x << 32) | z and leastSigBits = y;

## Fields
location: [Location](location.md) - location of the block

material: Material - material of the block

## Example
```json
{
  "location": {
    "world": "minecraft:overworld",
    "x": 0,
    "y": -60,
    "z": 0
  },
  "material": "minecraft:air"
}
```