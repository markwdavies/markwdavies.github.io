---
title: Amendment to WhatWasRestored SQL Proc
layout: default
---

# {{ page.title }}

Made a minor change to sp_WhatWasRestored proc today.  

The optional DBName parameter , if used , will now search for the name of the restored DB rather than the name of the DB that was backed up.