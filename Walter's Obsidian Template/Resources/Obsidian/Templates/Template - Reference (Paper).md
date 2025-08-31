---
up: "[[References]]"
date:
updated: 2025-08-30T11:57
journal: "[[2025-08-30]]"
category: Resource
type: Reference
status: Active
author:
publisher:
year:
source_type: Paper
url:
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
