---
title: WordPress Symbolic Link
date: 2024-03-03 10:00:00 -600
categories: [environments,installs,tools]
tags: [wordpress,packages,plugins,environments,tools,utilities]
---

# Creating WP Local Symbolic Link Environment

## Open both Local Engine folder of site and repo folder

1. Right click on the original repo select `pick link source`
2. Find local site directory folder, within `app/public` select `drop as symbolic link` within the folder
3. rename original `wp-content` to anything, this will act as backup
4. rename symbolic link folder to `wp-content`
5. navigate to original repo in vs code, navigate to `themes/rootrot` run `npm install`
6. activate the theme within wp-admin