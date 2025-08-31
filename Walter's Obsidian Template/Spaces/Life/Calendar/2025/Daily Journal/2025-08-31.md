---
up: "[[Journal Collection - 2025]]"
date: 2025-08-30
function: "1"
category: Life
type: Daily Journal
status: Active
Adventure:
image:
summary:
---

> [!info]-
>###### Previous Years:
>```dataview
>TABLE file.cday as "Created On"
>WHERE dateformat(file.cday, "MM-dd") = dateformat(this.file.day, "MM-dd")
>  AND regexmatch("\\d{4}-\\d{2}-\\d{2}", file.name)
>SORT file.cday ASC
>```
>
>###### Last Month:
>```dataview
>TABLE file.cday AS "Created On"
>WHERE dateformat(file.cday, "YYYY-MM-DD") = dateformat(this.file.day - dur(1 month), "YYYY-MM-DD")
>AND regexmatch("\\d{4}-\\d{2}-\\d{2}", file.name)
>SORT file.cday ASC
>```
>
>###### Last Week:
>```dataview
>TABLE file.cday AS "Created On"
>WHERE dateformat(file.cday, "YYYY-MM-DD") = dateformat(this.file.day - dur(7 days), "YYYY-MM-DD")
>AND regexmatch("\\d{4}-\\d{2}-\\d{2}", file.name)
>SORT file.cday ASC
>```
>
>###### Notes from Today:
>```dataview
>TABLE file.cday AS "Created On"
>WHERE date(file.cday) = date(today)
>SORT file.name ASC
>```

----

## Notes
- 


### Today's events
- 



## Photos
- 








-----
## Unrequited Links
```dataview
table file.mtime.year + "-" + file.mtime.month + "-" + file.mtime.day as Modified
from [[#]]
and !outgoing([[#]])
sort file.mtime desc
```
