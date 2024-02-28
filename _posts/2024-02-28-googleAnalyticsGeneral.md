---
title: Google Analytics - GA4 General
date: 2024-02-28 12:00:00 -600
categories: [analytics,google,SEO,GA4,installs,tools]
tags: [google,analytics,seo,ga4,packages,plugins,tools,utilities]
---

## Within `webmaster` account on Google Analytics
### Navigate to tag manager and use `webmaster` again
1. Create a new container, select respective use case (web for the most part), apply respective URL
2. Code is generated following creation of container
	2a. If this is within WPEngine and requires SFTP (Tturra e.g.) - go to respective site, underneath of the production side there will be `users and SFTP`
	> Will need to create an SFTP user if necessary, using respective FTP manager sign in using credentials
	2b. If within Elementor navigate to `Elementor` --> `Custom Code`, inject respective GA Tag code in Head/Body respective areas, save and publish (apply this change to entire site or specific page as necessary)
3.  Underneath of Tags `create new` --> Google Analytics --> GA4 Send an Event --> `measurement ID` is taken from `data connections`
4. `measurement ID` applied to new event, turn on `enhanced measurement`
5. Edit Event parameters within tag configuration and apply

### Create new Property
1. Select create new property
2. Select respective data stream (generate basic reports)
3. Provide website URL and stream name
4. Turn on enhanced measurement
5. `View tag instructions` button in top left, copy and paste code to be injected within Body or Head respectively
6. Ensure connection stream is working and test