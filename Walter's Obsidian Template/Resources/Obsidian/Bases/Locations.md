---
up: "[[Home]]"
date: 2025-08-29
updated: 2025-08-30T16:14
related: "[[People]]"
desc.: Collection of notes on places, regions, and environments, including their geography, features, and significance.
---

```base
filters:
  and:
    - file.folder == "Resources/Locations"
views:
  - type: table
    name: All
    order:
      - file.name
    sort: []
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```







## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
where !startswith(file.path, "Resources/Obsidian/Templates")
and !startswith(file.path, "Resources/Locations")
sort file.mtime desc
```







