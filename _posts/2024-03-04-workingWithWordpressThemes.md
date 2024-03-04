---
title: WordPress Themes Editing
date: 2024-03-04 12:00:00 -600
categories: [environments,installs,tools, themes]
tags: [wordpress,packages,plugins,environments,tools,utilities,themes]
---

# Working with Theme in WordPress and WordPress Local

1. Open Project
2. Navigate to files and have open to edit: `src/themes/project-name/src/sass/theme/components/respective-file.scss` also open `src/themes/project-name/template/created-item-file.php` also open `src/themes/project-name/archive-file.php`
3. Once files are open, resource file is made within WP-Admin in Advanced Custom Fields and creating a new post type, link respective items required of post type and save
4. Editing files or CSS of said components requires navigating from CLI to `c/repos/Project-Repo-Name/themes/project-name/src` and running `npm run watch`. This will compile and rebuild the SCSS to serve to the browser.
5. Additionally, WP Local must be running the site, and a Symbolic Link must have been established from the `site folder` within WP Local and your local repository.