---
up: "[[Home]]"
date: 2025-08-30
updated: 2025-08-30T16:14
desc.: Collection of notes that organize active and planned initiatives, each with defined goals, progress tracking, and outcomes.
---

```base
views:
  - type: table
    name: Active Projects
    filters:
      and:
        - file.folder == "Projects/Active"
    order:
      - file.name
      - date
      - desc.
    sort:
      - property: file.name
        direction: ASC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370
    columnSize:
      note.date: 120

```

-----

```base
views:
  - type: table
    name: Inactive Projects
    filters:
      and:
        - file.folder == "Projects/Inactive"
    order:
      - file.name
      - date
      - desc.
    sort:
      - property: file.name
        direction: ASC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370
    columnSize:
      note.date: 133

```



## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
where !startswith(file.path, "Resources/Obsidian/Templates")
and !startswith(file.path, "Projects")
sort file.mtime desc
```

