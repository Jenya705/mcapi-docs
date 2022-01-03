---
description: ->
    Description of ignores
---

Mcapi can ignore some classes on loading (e.g: route handlers). You can rule it with ignores.txt.
All ignorable classes has @Ignorable annotation on it. Just write class name in ignores.txt to ignore class or write directory like that `path.to.directory.*` or to ignore all ignorable objects (now is only routes) type `*`