<% '---' %>
<%*
let rawTitle = await tp.system.prompt('Enter the title:');

// Clean the title to make it a valid filename
let title = rawTitle
  .replace(/[\/\\:*?"<>|]/g, '')     // Remove invalid characters
  .replace(/\s+/g, ' ')              // Collapse multiple spaces
  .trim();                           // Remove leading/trailing spaces

let fileName = rawTitle.replace(/[\\/]/g, '-');

tR += "title: " + title + "\n";
await tp.file.rename(fileName);
%>
created_at: <% tp.file.creation_date('YYYY-MM-DD[T]HH:mm:ssZ') %>
modified_at: <% tp.file.last_modified_date('YYYY-MM-DD[T]HH:mm:ssZ') %>
category: Bible
type: Scripture
topic:
  - Scripture
tags:
  - bible/verse
  - bible/book/
status: Active
<% '---' %>
# `= this.title`

> [[🏠 Homepage]]
---