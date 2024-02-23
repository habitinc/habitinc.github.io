---
title: Installing and Running Jekyll and Ruby (Windows)
date: 2024-02-22 12:00:00 -600
categories: [languages,installs]
tags: [jekyll,ruby]
---

# Jekyll Chirpy Project Install
## Repo and theme of base project: [Link Text](https://github.com/cotes2020/jekyll-theme-chirpy)

1. Install ruby at [Link Text](https://rubyinstaller.org/)
2. Run IN POWERSHELL or Admin terminal (windows) `gem -v` to check version of gem is installed correctly
3. Run `gem install bundler`
4. Run `bundle`

To then run local server:
1. Run command `bundle exec jeykll s`

To edit Globals:
- File `_config.yml`

To create Content:
- Within folder `posts`
	-> Utilizes markdown syntax
	-> Create post by creating file within `posts` of `fileName.md`
	-> Ensure posts are created with file name of `2024-XX-XX-filename.md`
	-> Save and push your changes to repo (main branch)