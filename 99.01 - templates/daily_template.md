---
creation date: <% tp.file.creation_date() %>
last modified: <% tp.file.last_modified_date() %>
tags: DailyNote <% tp.file.title.split('-')[0] %> <% tp.file.title.split('-')[1] %>
---

# <% tp.file.title %>

<< [[<% tp.date.now("YYYY.MM.DD", -1, tp.file.title, "YYYY.MM.DD") %>]] | [[<% tp.date.now("YYYY.MM.DD", 1, tp.file.title, "YYYY.MM.DD") %>]]>>

# Tasks
## Over Due
```tasks
not done
due before <% tp.file.title.split('-')[0] %>-<% tp.file.title.split('-')[1] %>-<% tp.file.title.split('-')[2] %>
short mode
```

## Due Today
```tasks
not done
due on <% tp.file.title.split('-')[0] %>-<% tp.file.title.split('-')[1] %>-<% tp.file.title.split('-')[2] %>
path does not include <% tp.file.path(true) %>
short mode
```

## New Today
- [ ] 

---
# PARA
## Projects
- 

## Areas
- Danish::
- Reading:: 
- Water::
- Exercise::

## Research
- 

## Archived
- 
---
# Meeting Log
## 0800: 

---
# Other Tasks

#### Done Today
```tasks
done on <% tp.file.title.split('-')[0] %>-<% tp.file.title.split('-')[1] %>-<% tp.file.title.split('-')[2] %>
```

#### No Due Date
```tasks
not done
no due date
```
---
