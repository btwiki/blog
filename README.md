# Braintrust Blog

## Editing guidelines
Modifications should only ever have to be made in the `/_posts/` and `/_tags/` directories under normal circumstances.  
To add a new post, create a file with the name structure `YYYY-MM-DD-simple-name.md` and insert into it the following header:
```yaml
---
layout: post
author: your-name
title: The post title!
description: Something descriptive
summary: Something short
tags: [any, tags]
usemathjax: true
---
```
Replacing the relevant fields as necessary.

If you wish to tag a post with a tag that does not currently exist in `/_tags/`, create a new file for the tag  
named exactly the same, such as `blog.md` for the tag `blog`, and insert into it *only these lines*:

```yaml
---
layout: tag
tag: tag-name
---
```
Again, replacing the tag-name as necessary.