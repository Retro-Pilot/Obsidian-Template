---
up: "[[Home]]"
related: "[[Adventure Collection - 2025]]"
category: Life
type: Collection
status: Active
---
`button-Today`

-----

```base
filters:
  and:
    - file.folder == "Spaces/Life/Calendar/2025/Daily Journal"
views:
  - type: cards
    name: .
    order:
      - file.name
      - summary
      - image
    sort:
      - property: file.name
        direction: DESC
    fields:
      - file.name
      - desc
      - updated
    cardSize: 190
    columnSize:
      note.summary: 438
    image: note.image
    imageAspectRatio: 0.35
    imageFit: ""

```




