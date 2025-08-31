---
up: "[[Home]]"
date: 2025-08-29
updated: 2025-08-31T11:28
desc.: Personal log of books to read, track progress on, and record viewing notes.
---


```base
filters:
  and:
    - file.folder == "Resources/Media/Books"
views:
  - type: table
    name: Reading
    filters:
      and:
        - status == "Reading"
    order:
      - file.name
      - author
    sort:
      - property: file.name
        direction: ASC
      - property: date
        direction: ASC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

---

```base
filters:
  and:
    - file.folder == "Resources/Media/Books"
views:
  - type: table
    name: Later
    filters:
      and:
        - status == "Later"
    order:
      - file.name
      - author
    sort:
      - property: file.name
        direction: ASC
      - property: date
        direction: ASC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

---
```base
views:
  - type: table
    name: Completed
    filters:
      and:
        - file.folder == "Resources/Media/Books"
        - status == "Completed"
    order:
      - file.name
      - author
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





## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
where !startswith(file.path, "Resources/Obsidian/Templates")
and !startswith(file.path, "Resources/Media/Books")
sort file.mtime desc
```

