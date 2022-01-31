---
description: >-
    Description of item stack rest object
---

## Fields
material: String - The item material

amount: Integer - The item amount

customName: Optional Component - The item custom name. Empty if item does not have custom name

enchantments: Optional List of Item Enchantments - The item enchantments. Empty if item does not have any enchantments.

## Example
```json
{
  "material": "minecraft:stick",
  "amount": 1,
  "customName": {
    "text": "Invisible stick"
  }
}
```