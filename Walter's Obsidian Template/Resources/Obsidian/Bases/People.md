---
up: "[[Home]]"
date: 2025-08-29
updated: 2025-08-30T16:14
related: "[[Locations]]"
desc.: Collection of notes on people, including historical figures, public individuals, and personal contacts, with focus on their lives, roles, and relationships.
---

```base
filters:
  and:
    - file.folder == "Resources/People/Personal"
views:
  - type: table
    name: Personal
    order:
      - file.name
    sort:
      - property: file.name
        direction: DESC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

-----

```base
views:
  - type: table
    name: Public
    filters:
      and:
        - file.folder == "Resources/People/Public"

```





## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
where !startswith(file.path, "Resources/Obsidian/Templates")
and !startswith(file.path, "Resources/People")
sort file.mtime desc
```
















