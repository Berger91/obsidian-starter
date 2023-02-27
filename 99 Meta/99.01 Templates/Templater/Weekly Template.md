---
title: <% tp.file.title %>
created: <% tp.file.creation_date() %>
aliases:
tags:
- '#weekly-note'
date: <% tp.file.creation_date() %>
endDate: <% tp.date.now("YYYY-MM-DD", 6) %>
---

# Weekly note <% tp.date.now("YYYY-MM-DD") %> - <% tp.date.now("YYYY-MM-DD", 6) %>

## Expedite

## Every Day Tasks
- Change Weely template and add whatever you want


## Read It Later

Limited to 10 elements
```dataview
TABLE file.name as "Name", file.ctime as "Created" FROM "00 Inbox/00.03 ReadItLater Inbox"
SORT file.ctime DESC
LIMIT 10
```

## Not finished Tasks

This query lists not finished tasks from previous weekly notes
```dataview
TASK FROM "10 Weekly Log"
WHERE !completed
SORT file.ctime DESC
LIMIT 20
GROUP BY file.ctime
SORT rows.file.ctime DESC
```
