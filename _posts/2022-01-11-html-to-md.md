---
layout: post
title: HTML to MD with Python
---

{{ page.title }}
================

<!--Available Meta Tags: Windows, Scripting, Productivity, Context Menu, Shortcuts, Dev Tools, Utility, Software Development, Code, Tutorial, Automation, Design, Adobe, Software, Excel, Bookmarklet, Graphics, Analysis, Sorting, Marketing -->
<p class="meta">Windows, Scripting, Productivity, Dev Tools, Utility, Code</p>

![HTML to MD](/images/-htmlmd.png)
{: #hero}

## Make an HTML to Markdown converter with Python

---

- Make an html page with all elements
- Python convert html to md equal element-code
- Save as '.md'

```
import re

txt = "<h1>Headline H1</h1>"
x = re.search("^<h1>.*</h1>$", txt)
```
