---
description: >-
    List of all events
---

* [player_join](#playerjoin)
* [player_link](#playerlink)
* [menu_click](#menuclick)
* [chat_message](#chatmessage)
* [player_block_break](#playerblockbreak)
* [player_block_place](#playerblockplace)
* [player_quit](#playerquit)
* [subscribe](#subscribe)
* [player_unlink](#playerunlink)
* [inventory_move](#inventory_move)

## PlayerJoin

Join event is called everytime when player joins to the server.

### Fields
player: Player - player who joined

## PlayerLink

Link event is called everytime when player declines or accepting bot link

### Fields
failed: Boolean - is link failed

player: UUID - player uuid

declinePermission: Array of strings - declined optional permissions


### MenuClick

Menu click event is called everytime when player clicks bot inventory

### Fields
id: String - bot inventory id

player: Player - player, who clicked

## ChatMessage

Message event is called everytime when player type the message

### Fields

message: String - player message

author: UUID - author uuid

## PlayerBlockBreak

Block break event is called everytime when player breaks the block

### Fields
player: Player - player, who broke the block

brokenBlock: Block - block, which was broken

## PlayerBlockPlace

Block place event is called everytime when player places the block

### Fields
player: Player - player, who placed the block

placedBlock: Block - block, which was placed

## PlayerQuit

Quit event is called everytime when player quits the server

### Fields
player: Offline player - player who quit

## Subscribe

Subscribe event is response to event tunnel subscription

### Fields
failed: array of strings - failed subscriptions

## PlayerUnlink

Unlink event is called when player unlinks with bot

### Fields
player: UUID - player uuid

## Inventory Move

### Fields
destinationSlot: Optional Integer - destination slot. Empty if no destination slot (e.g. air)

sourceSlot: Optional Integer - source slot. Empty if no source slot.

item: ItemStack - moved item.

destination: Optional InventoryHolder - destination inventory holder. Empty if no destination inventory (e.g. air)

source: Optional (InventoryHolder or String) - source inventory holder. "destination" if source inventory is destination inventory. Empty if no source inventory.

initiator: Optional (InventoryHolder or String) - initiator inventory holder. "destination" if initiator inventory is destination inventory or "source" if initiator inventory is source inventory. Empty if no initiator.