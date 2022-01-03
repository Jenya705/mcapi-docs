---
description: ->
    Description of link ignores
---

Rule permission which can be requested on linking state. write permission without `-` to allow it, and with to disallow it. Write `permission.a.*` to allow all sub permission to be allowed or `-permission.a.*` to disallow all sub permissions. If permission allowed so it is not disallowed, so if you write
```
some.permission
-*
```
`some.permission` will be allowed, but all others won't