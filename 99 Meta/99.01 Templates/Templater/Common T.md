---
title: <% tp.file.title %>
created: <% tp.file.creation_date() %>
tags:
  - '#<% tp.file.find_tfile(tp.file.title).path.replace(`/${tp.file.title}.md`,'').split('/').join("\'\n  - \'#") %>'
directory: <% tp.file.find_tfile(tp.file.title).path.replace(`/${tp.file.title}.md`,'') %>
---

# <% tp.file.title %>