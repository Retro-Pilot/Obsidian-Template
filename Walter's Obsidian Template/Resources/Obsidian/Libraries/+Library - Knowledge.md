---
up: "[[Home]]"
date: 2025-08-29
updated: 2025-08-30T16:14
type: Library
desc.: Collection of MOCs that organize fields of study, external knowledge, and subjects of curiosity and learning.
---

----
## Creativity & Expression

```base
filters:
  and:
    - file.folder == "Spaces/Knowledge/MOCs/Creativity and Expression"
views:
  - type: table
    name: .
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

----
## Outdoors
```base
filters:
  and:
    - file.folder == "Spaces/Knowledge/MOCs/Outdoors"
views:
  - type: table
    name: .
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


---
## Science & Technology

```base
filters:
  and:
    - file.folder == "Spaces/Knowledge/MOCs/Science & Technology"
views:
  - type: table
    name: .
    order:
      - file.name
    sort:
      - property: file.name
        direction: ASC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 190
    imageFit: ""

```

---
## Society & Systems

```base
filters:
  and:
    - file.folder == "Spaces/Knowledge/MOCs/Society and Systems"
views:
  - type: table
    name: .
    order:
      - file.name
    sort: []
    fields:
      - file.name
      - desc
      - updated

```

