


```
---
title:"<% tp.file.title %>"
author: BCN.LI
type: post
date: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ssZ") %>
lastmod: <% tp.file.last_modified_date("YYYY-MM-DDTHH:mm:ssZ") %>
url: <% tp.file.creation_date("/YYYY/MM/DD/") %><% tp.file.title.toLowerCase().replaceAll(" ", "-") %>
excerpt: <% tp.system.prompt("Enter excerpt", "") %>
categories:
<%*
    let categories = await tp.system.prompt("Enter categories, comma separated", "")
    console.log(categories)
    categories = categories.toLowerCase().split(",").map(val => `  - ${val}`).join("\n")
%><% categories %>
tags:
<%*
    let tags = await tp.system.prompt("Enter tags, comma separated", "")
    console.log(tags)
    tags = tags.toLowerCase().split(",").map(val => `  - ${val}`).join("\n")
%><% tags %>
---
```
---
[[- InternetScrap]]
