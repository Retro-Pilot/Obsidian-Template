---
up: "[[Home]]"
date: 2025-08-29
updated: 2025-08-30T16:14
type: Library
desc.: Collection of MOCs and notes that organize personal systems, daily practices, and lived experience.
---


---
## Finances

```base
filters:
  and:
    - file.folder == "Spaces/Life/MOCs/Finances"
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
## Health

```base
filters:
  and:
    - file.folder == "Spaces/Life/MOCs/Health"
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
    cardSize: 370

```

---
## Household

```base
filters:
  and:
    - file.folder == "Spaces/Life/MOCs/Household"
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
## Misc

```base
filters:
  and:
    - file.folder == "Spaces/Life/MOCs/Misc"
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
    cardSize: 370

```

---
## Outdoors

```base
filters:
  and:
    - file.folder == "Spaces/Life/MOCs/Outdoors"
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




