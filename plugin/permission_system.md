---
description: >-
    Description of mcapi permission system
---

All permissions have two types - global and target. 
* Global permission affects on all targets (for now only players). 
* Target permission affects only on specific player.

If no target permission specified, global permission will be used. 
If no global and target permission specified, default value will be used (can be specified in `storage` config file) <br>

`some.perm.*` will affect on all sub permissions (example: `some.perm.perm`, `some.perm.another`)

## How to set permission
Use `/mcapi bot permission give` command 

