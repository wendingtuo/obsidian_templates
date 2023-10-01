---
creation date: <% tp.file.creation_date() %>
tags:
  - Periodic_Notes/Daily_Note
week: W{{date:w-yyyy}}
TimeIn: 
TimeOut: 
TimeTotal:
---
<%* const dow = moment(tp.file.title, "YYYY-MM-DD").format("dd");-%>
<%* if (dow == "ma") {  -%>
<< [[<% moment(tp.file.title, 'YYYY-MM-DD').subtract(3, 'd').format('YYYY-MM-DD') %>]] | [[<% moment(tp.file.title, 'YYYY-MM-DD').add(1, 'd').format('YYYY-MM-DD') %>]] >>
<%* } else if (dow == "fr") {  -%>
<< [[<% moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>]] | [[<% moment(tp.file.title, 'YYYY-MM-DD').add(3, 'd').format('YYYY-MM-DD') %>]] >>
<%* } else if (dow != "ma" && dow != "fr") {  -%>
<< [[<% moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>]] | [[<% moment(tp.file.title, 'YYYY-MM-DD').add(1, 'd').format('YYYY-MM-DD') %>]] >>
<%* } else {} -%>
___
## Journal

- 

## PARA
### In Progress
```dataview
TABLE dateformat(file.mtime, "dd.MM.yyyy - HH:mm") AS "Modified"
from #Status/In_Progress
sort file.mtime desc
```

### Responsibilities
```dataview
TABLE dateformat(file.mtime, "dd.MM.yyyy - HH:mm") AS "Modified"
from #Status/Responsibilities 
sort file.mtime desc
```

### On Hold
```dataview
TABLE dateformat(file.mtime, "dd.MM.yyyy - HH:mm") AS "Modified"
from #Status/On_Hold 
sort file.mtime desc
```

### Recent Notes
```dataview
TABLE dateformat(file.mtime, "dd.MM.yyyy - HH:mm") AS "Modified"
FROM !"00 - Daily Notes" AND !"99 - Meta" AND !#Status/In_Progress AND !#Status/On_Hold
WHERE date(<% moment(tp.file.title, 'YYYY-MM-DD').format('YYYY-MM-DD') %>) - file.mtime <= dur(7 days)
WHERE file.name != this.file.name
SORT file.mtime DESC
```
