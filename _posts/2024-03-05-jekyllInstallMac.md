---
title: Installing and Running Jekyll and Ruby (Mac)
date: 2024-03-05 12:00:00 -600
categories: [languages, installs]
tags: [jekyll, ruby]
---

# Jekyll Chirpy Project Install

## Repo and theme of base project: [Link Text](https://github.com/cotes2020/jekyll-theme-chirpy)

1. Install ruby at [https://jekyllrb.com/docs/installation/](https://jekyllrb.com/docs/installation/)
2. Run terminal `ruby -v` to check if it's installed correctly
3. Clone the Habitinc.github.io repo to your local machine

To then run local server:

1. Run `bundle`
2. Run `jekyll serve`
   - if you run into a port in use error run `jekyll serve -P portnumber` to change the port being used

To edit Globals:

- File `_config.yml`

To create Content:

- Within folder `posts`
  -> Utilizes markdown syntax
  -> Create post by creating file within `posts` of `fileName.md`
  -> Ensure posts are created with file name of `2024-XX-XX-filename.md`
  -> Save and push your changes to repo (main branch)
