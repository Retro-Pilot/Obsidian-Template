---
up: "[[Home]]"
date: 2025-08-30
updated: 2025-08-31T11:28
desc.: Personal log of shows and movies to watch, track progress on, and record viewing notes.
---

```base
views:
  - type: table
    name: Watching
    filters:
      and:
        - file.folder == "Resources/Media/Movies and TV"
        - status == "Watching"
    order:
      - file.name
      - date
      - desc.
    sort:
      - property: file.mtime
        direction: DESC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370
    columnSize:
      note.date: 120

```

---

```base
views:
  - type: table
    name: Later
    filters:
      and:
        - file.folder == "Resources/Media/Movies and TV"
        - status == "Later"
    order:
      - file.name
      - date
      - desc.
    sort:
      - property: file.mtime
        direction: DESC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370
    columnSize:
      note.date: 120

```

---

```base
views:
  - type: table
    name: Completed
    filters:
      and:
        - file.folder == "Resources/Media/Movies and TV"
        - status == "Completed"
    order:
      - file.name
      - date
      - desc.
    sort:
      - property: file.mtime
        direction: DESC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370
    columnSize:
      note.date: 120

```





## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
where !startswith(file.path, "Resources/Obsidian/Templates")
and !startswith(file.path, "Resources/Media/Movies and TV")
sort file.mtime desc
```

