---
creation date: <% tp.file.creation_date() %>
last modified: <% tp.file.last_modified_date() %>
tags: WeeklyNote <% tp.file.title.split('-')[0] %> <% tp.file.title.split('-')[1] %>
---

# <% tp.file.title %> - Weekly Summary

## Startup
- [ ] Transpose Meetings & Appointments
- [ ] Set Goals
- [ ] Move Items from backlog into todo that will help accomplish goals

## Planned Tasks
Actions that will ensure I make progress on my goals
- 

___
## Week at a Glance
[[<% tp.file.folder(true) %>/{{monday:YYYY-MM-DD - dddd}}|Monday]]
[[<% tp.file.folder(true) %>/{{tuesday:YYYY-MM-DD - dddd}}|Tuesday]]
[[<% tp.file.folder(true) %>/{{wednesday:YYYY-MM-DD - dddd}}|Wednesday]]
[[<% tp.file.folder(true) %>/{{thursday:YYYY-MM-DD - dddd}}|Thursday]]
[[<% tp.file.folder(true) %>/{{friday:YYYY-MM-DD - dddd}}|Friday]]
[[<% tp.file.folder(true) %>/{{saturday:YYYY-MM-DD - dddd}}|Saturday]]
[[<% tp.file.folder(true) %>/{{sunday:YYYY-MM-DD - dddd}}|Sunday]]

___
## End Of Week Review
-   What did I get done this week versus what I planned to get done?
-   What unexpectedly arose this week that blocked my productivity?
-   What worked well?
-   Where did I get stuck?
-   What did I learn?
-   When did I feel most energized?

___
## Weekly Task Review
```tasks
path includes <% tp.file.folder(true) %>
sort by status
sort by priority
```
