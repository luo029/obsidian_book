[!abstract] [Page <%= it.pageLabel %>](<%= it.backlink %>)
<mark style="<%- if (it.color) { _%> color: <%= it.color %>; <%_ } -%><%- if (it.bgColor) { _%> background-color: <%= it.bgColor %>; <%_ } -%>"><%= it.imgEmbed %><%= it.text %><img src="/i/mouse.jpg" ==height="200" width="200"== /></mark><% if (it.comment) { %>
* * *

<%= it.comment %><% } %>