
# <%= it.title %>


```ad-info
- **Authors**: <%=
it.authors
.map(author => `[[${author}]]`)
.join(', ')
%>
- **Date**: <%= it.date ?? it.year %>
- **ISBN**: <%= it.ISBN %>
- **Groups**: <%= it.collections %>
- **Tags**: <%=
it.tags
.map(tag => `#` + tag.toString().replaceAll(' ', '-'))
.join(', ')
%>
- **Links**：[Zotero](<%= it.backlink %>), <%= it.fileLink %>
- **Path** : <%=it.attachment.path %>
```

<% it.notes.forEach(note => { -%>
<%= `${note}` %>
<% }) %>
# 注释
<%~ include("annots", it.annotations) %>