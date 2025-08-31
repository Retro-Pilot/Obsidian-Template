---
up: "[[Home]]"
related: "[[Journal Collection - 2025]]"
updated: 2025-08-31T00:18
category: Life
type: Journal
status: Draft
desc.: Log of personal outdoor trips and experiences, capturing routes, memories, and reflections.
---



```base
filters:
  and:
    - file.folder == "Spaces/Life/Calendar/2025/Daily Journal"
    - Adventure == true
views:
  - type: cards
    name: .
    order:
      - file.name
      - summary
      - image
    sort: []
    fields:
      - file.name
      - desc
      - updated
    cardSize: 210
    columnSize:
      note.summary: 419
    image: note.image
    imageFit: contain

```



