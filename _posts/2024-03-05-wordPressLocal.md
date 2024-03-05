---
title: Setting up a WordPress Website Locally
date: 2024-03-05 12:00:00 -600
categories: [wordpress]
tags: [wordpress, themes, local]
---

You may need to use a local version of a WordPress theme in order to make/test codebase changes, using [LocalWP](https://localwp.com/), you will be able to set up a local WordPress Environment with a few clicks.
Before following the steps below, install LocalWP

## Setup an Environment

1. Click the + icon to create a new site
2. Choose the `Create a new site` option
3. Name the site
4. Used the `Preferred` setting or `Custom` if you need to adjust something
5. Create a Dashboard login
6. Click `Add Site`

## Import a Theme into the Environment

1. Click the `Go to site folder` option within the environment
2. Navigate to `app > public`
3. Rename the `wp-content` folder
4. Create a [symlink](/posts/wordPressSymbolicLink/) of the theme's repo
5. Drop the symlink'd folder into the local environment directory in step 2
6. Rename the symlink'd folder to `wp-content`
   - Run `npm install` on the repo if you have not already to populate the theme
7. Login to the local environment
8. In the Appearance Panel, select the working theme
