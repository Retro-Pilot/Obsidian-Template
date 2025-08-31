---
up: "[[Home]]"
date: 2025-08-29
updated: 2025-08-30T16:14
desc.: Collection of external sources such as articles, books, manuals, and papers, preserved for study, citation, and future use.
---

```base
filters:
  and:
    - file.folder == "Resources/References/Articles"
views:
  - type: table
    name: Articles
    order:
      - file.name
    sort: []
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

```base
filters:
  and:
    - file.folder == "Resources/References/Manuals"
views:
  - type: table
    name: Manuals
    order:
      - file.name
    sort: []
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

```base
filters:
  and:
    - file.folder == "Resources/References/Papers"
views:
  - type: table
    name: Research Papers
    order:
      - file.name
    sort: []
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

```base
filters:
  and:
    - file.folder == "Resources/References/Quotes"
views:
  - type: table
    name: Quotes
    order:
      - file.name
    sort: []
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

```base
filters:
  and:
    - file.folder == "Resources/References/Social"
views:
  - type: table
    name: Social Posts
    order:
      - file.name
    sort: []
    fields:
      - file.name
      - desc
      - updated
    cardSize: 370

```

```base
filters:
  and:
    - file.folder == "Resources/References/Video"
views:
  - type: table
    name: Videos
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
and !startswith(file.path, "Resources/Bookmarks")
sort file.mtime desc
```



