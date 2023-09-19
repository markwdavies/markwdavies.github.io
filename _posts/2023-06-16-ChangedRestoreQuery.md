---
title: Amendment to WhatWasRestored SQL Proc
layout: post
tags: news sql
---

# {{ page.title }}

Made a minor change to the sql to create the **sp_WhatWasRestored** proc today.  

The optional **@DBName** parameter , if used , will now search for the name of the restored DB rather than the name of the DB that was in the source backup set.
