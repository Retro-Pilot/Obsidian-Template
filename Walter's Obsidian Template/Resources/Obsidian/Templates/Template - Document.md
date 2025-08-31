---
up: "[[Documents]]"
date: 2025-08-30
updated: 2025-08-30T11:56
journal: "[[2025-08-30]]"
category: Life | Resources
type: Document
status: Active
doc_type:
related:
desc.:
---
















-----
## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
sort file.mtime desc
```
