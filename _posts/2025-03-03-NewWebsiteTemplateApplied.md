---
title: Website rewritten with New Theme
layout: post
tags: news misc
author: mwd
---
# {{ page.title }}
This Github Pages hosted website has now been rewritten by applying the [Hacker Theme](https://github.com/pages-themes/hacker) for Jekyll.

This was straightforward to do following the documentation and links from the GitHub Pages Hosting and Jekyll websites. 
- - - 
### Test Locally
To avoid the code bloat that would result from testing the site on my local machine I created a test VM and used this to build and remotely test the site before deploying to GitHub. The steps I took to do this were :

1. Install VMware fusion, which is now [free for personal use](https://blogs.vmware.com/teamfusion/2024/05/fusion-pro-now-available-free-for-personal-use.html).
2. Install  Debian on a new VM using a free download of [Debian](https://www.debian.org/distrib/).
3. Install git on the new VM using the Debian software manager.

- - -
### Amend site
Next I followed the GitHub instructions for installing the software to [test locally](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).

I also cross referenced to [Jekyll documentation](https://jekyllrb.com/docs/) for more detailed explanations.
- - -
### Deploy
Once all set up , I pulled the existing site from Github. Then applied the new Theme as per [Github Pages instructions](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll) then rebuilt the site locally to test on my Debian VM.

There was some re-editing required of the templates and posts but once complete, I committed the changes locally in git and pushed it back to Github where it was automatically rebuilt and deployed in its new format.
