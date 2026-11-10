---
DM:
players:
  -
characters:
  -
---

Sessions
```dataview
TABLE session, location
FROM #session
WHERE contains(this.file.inlinks, file.link)
SORT session
```
