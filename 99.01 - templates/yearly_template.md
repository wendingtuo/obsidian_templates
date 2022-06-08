---
creation date: <% tp.file.creation_date() %>
last modified: <% tp.file.last_modified_date() %>
tags: YearlySummary <% tp.file.title.split('.')[0] %>
---

# <% tp.file.title %> - Yearly Summary
## Task Review
---
#### Done This Year
```tasks
done
path includes <% tp.file.folder(true) %>
short mode
sort by done
```

#### Due This Year
```tasks
not done
path includes <% tp.file.folder(true) %>
sort by priority
```

