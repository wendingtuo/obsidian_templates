---
creation_date: <% tp.file.creation_date() %>
tags: Periodic_Notes/Weekly_Note
week: W{{date:w-yyyy}}
---
## Weekly Time Review

```dataview
TABLE TimeTotal
FROM "00 - Daily Notes"
WHERE TimeTotal
WHERE week = "<% tp.file.title.split('-')[1] %>-<% tp.file.title.split('-')[0] %>"
SORT Date asc
```

## End Of Week Review

-  [ ] Complete Time Sheet
-  [ ] Complete Weekly Review
	- What did I get done this week versus what I planned to get done?
	- What unexpectedly arose this week that blocked my productivity?
	- What worked well?
	- Where did I get stuck?
	- What did I learn?
	- When did I feel most energized?

## Week at a Glance


![[<% tp.file.folder(true) %>/{{monday:YYYY-MM-DD }}#Journal]]

---
![[<% tp.file.folder(true) %>/{{tuesday:YYYY-MM-DD}}#Journal]]

---
![[<% tp.file.folder(true) %>/{{wednesday:YYYY-MM-DD}}#Journal]]

---
![[<% tp.file.folder(true) %>/{{thursday:YYYY-MM-DD}}#Journal]]

---
![[<% tp.file.folder(true) %>/{{friday:YYYY-MM-DD}}#Journal]]

---
