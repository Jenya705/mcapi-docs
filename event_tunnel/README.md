---
description: >-
    Description of mcapi event tunnel
---

Event tunnel is a mechanism to handle events threw websocket.

## Object

Event tunnel object always have `type` field of type string  

## Compression

All objects is compressed using zlib (Sended and received)

## Connect

### Authorization

To authorize you need to send authorization request. It is contain one field `token` with bot token

```json
{"token":"8f5b10c0e94e4693a1258de63a51fe1f0000001642336264452"}
```

### Subscribe

To subscribe to events you need to send subscribe request. It is need to be send after authorization. Request contains field `subscriptions` with list of events

```json
{"subscriptions":["message", "command_interaction", "link", "unlink", "join", "quit", "block_place", "captured_entity_click", "menu_click"]}
```