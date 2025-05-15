---
title: Updated WhatIsRunning SQL Proc
layout: post
tags: news sql
---
# {{ page.title }}
It's been a while since anything has changed so I've a couple of minor changes to the **sp_WhatIsRunning** proc.

A couple of optional parameters have been added to the stored proc to narrow down the output.  Both default to a value of 0 , set them to 1 to affect the output. 

Use the **ActiveOnly** parameter to limit output to currently running sessions.
Use the **@BackupsOnly** parameter to only show backups and restores.

e.g. `EXEC sp_WhatIsRunning @ActiveOnly = 0 , @BackupsOnly = 1`

I've also added percentage completion to the output - this only contains a value for a few commands , such as backup and restore and DBCC CHECKDB. It gives no indication of how much longer the task will take to complete but it can be good to know that some progress has been made !!

That's all for now :-)  