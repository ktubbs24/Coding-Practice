---
banner_icon: ⌨️
banner: "![[blue binary code image.jpg]]"
banner_y: 0.936
date: 2025-08-30T03:31:00
status:
  - archived
---
# Home 
---
<iframe src="https://jandee.vercel.app/ktubbs24" width="100%" height="300" frameborder="0"></iframe>

## </> Devlog 
```dataview
TABLE date, platforms, languages
FROM "1-Practice/Daily Devlogs"
WHERE type = "devlog"
SORT date DESC
```






## </> By Status 
```dataview
LIST
FROM ""
WHERE status = "learning"
SORT level ASC
```


## </> Progress Tracker 
```dataview 
TABLE language, topic, last-practiced
FROM "1-Practice"
WHERE status != "archived"
SORT last-practiced DESC
```

## </> Last Practice Based On Topic 
*below example is filtering out for now loops*

```dataview
TABLE related
WHERE topic = "loops"
```

## </> Last Practiced Based On Language
```dataview 
TABLE type, topic, status, last-practiced
FROM ""
WHERE language
SORT last-practiced DESC
```


## </> Devlog Overview 

![[Devlog and Notes.base]]