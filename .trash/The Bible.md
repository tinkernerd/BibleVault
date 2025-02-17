---
title: The Bible
description: A dashboard for organizing Bible notes, books, and verses.
tags:
  - bible
  - dashboard
  - dash/personal
  - homepage
  - followup
banner-display: cover
type: Dashboard/L1
category: Bible
banner: https://unsplash.com/photos/UIib0bAvWfs/download?ixid=M3wxMjA3fDB8MXxhbGx8fHx8fHx8fHwxNzM5NzUzOTg4fA&force=true
banner-height: 270
banner-x: 58
banner-y: 41
---
## 📚 Bible Notes
### UnSorted Notes
```dataview
TABLE WITHOUT ID  
link(file.path, title) AS "Note", file.mtime AS "Last modified"
FROM "Notes"
WHERE contains(category, "Bible") AND contains(type, "Scripture")
SORT title ASC
```
### Bookmarked
- [[Verse Book]]
### 📚 Testaments
- [[Old Testament Overview]]
- [[New Testament Overview]]
### Reflection Notes
```dataview
TABLE WITHOUT ID  
link(file.path, title) AS "Note", created_at as "Date Created", file.mtime AS "Last modified"
FROM "Notes"
WHERE contains(category, "Bible") AND type = "Reflection"
SORT title ASC
```
### Sermons
```dataview
TABLE WITHOUT ID  
link(file.path, title) AS "Note", type AS Type, created_at AS "Date Created"
FROM "Notes"
WHERE contains(category, "Bible") AND type = "Sermon" 
SORT title ASC
```
### Bible Study Notes
```dataview
TABLE WITHOUT ID  
link(file.path, title) AS "Note", type AS Type, created_at AS "Date Created"
FROM "Notes"
WHERE contains(category, "Bible") AND type = "Bible Study" 
SORT title ASC
```
