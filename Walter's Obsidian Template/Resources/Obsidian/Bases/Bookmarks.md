---
up: "[[Home]]"
date: 2025-08-29
updated: 2025-08-30T16:14
desc.: Personal collection of saved links, articles, and resources for quick access and future reference.
---

```base
filters:
  and:
    - file.folder == "Resources/Bookmarks"
views:
  - type: table
    name: All
    order:
      - file.name
    sort:
      - property: file.name
        direction: ASC
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
and !startswith(file.path, "Resources/Bookmarks")
sort file.mtime desc
```



