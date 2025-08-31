---
up: "[[Home]]"
date: 2025-08-30
updated: 2025-08-31T11:32
journal: "[[2025-08-30]]"
category:
type:
status: Active
related:
---













-----
## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
sort file.mtime desc
```
