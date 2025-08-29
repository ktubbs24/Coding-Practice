# Home
---







## By Status 
```dataview
LIST
FROM ""
WHERE status = "learning"
SORT level ASC
```


## Progress Tracker 
```dataview 
TABLE language, topic, last-practiced
FROM "1-Practice"
WHERE status != "archived"
SORT last-practiced DESC
```


## Last Practice Based On Topic 
*below example is filtering out for now loops*

```dataview
TABLE related
WHERE topic = "loops"
```

## Last Practiced Based On Language
```dataview 
TABLE type, topic, status, last-practiced
FROM ""
WHERE language
SORT last-practiced DESC
```


## Overview 

![[Code Database.base]]