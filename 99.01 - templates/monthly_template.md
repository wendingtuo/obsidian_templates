---
creation date: <% tp.file.creation_date() %>
last modified: <% tp.file.last_modified_date() %>
tags: MonthlyNote <% tp.file.title.split('-')[0] %> <% tp.file.title.split('-')[1] %>
---

# <% tp.file.title %> - Monthly Summary

## Monthly Goals
___ 
- [ ] 


## Monthly Checklist
---
### Start of Month
- [ ] Check Email
- [ ] Check Teams
- [ ] Check showing online
- [ ] Check Calendar - Time Block

### End of Month
- [ ] Show Offline
- [ ] Clean Unused Headings in Daily Log
- [ ] Check tomorrow's calendar

## Monthly Task Review
---
#### Done This Month
```tasks
done
path includes <% tp.file.folder(true) %>
short mode
sort by done
```

#### Due This Month
```tasks
not done
path includes <% tp.file.folder(true) %>
sort by priority
```

