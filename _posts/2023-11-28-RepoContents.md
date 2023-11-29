---
title: SQL Server Stored Procedures
layout: post
tags: sql
author: mwd
---

# {{ page.title }}
## in my GitHub repo 

The [Stored Procs github repo](https://github.com/markwdavies/SQLServerUtilities/tree/main/StoredProcs) currently contains the following scripts.

Each script, by default, creates the Stored Procedure in the Master database from where it can be run, each script will replace a like named Stored proc if one has already been created.

The __RemoveStoredProcs.sql__ script will remove from the Master database any stored procs created with the same names as those in the repository. This is only needed if tidying up the master DB.

***
* __WhatIsRunning.sql__ 
    * Display details of running sessions. 
    * Usage : `EXEC sp_WhatIsRunning`

***
* __WhatWasBackedUp.sql__
    * Display details of latest Database Backups for each DB on current instance. 
    * Use optional `@DBName` parameter to narrow down results to a specific DB or a subset using wildcards.
    * Use optional `@FullBackupsOnly` parameter with a value of 1 to restrict results to Full Backups.
    * Usage : `EXEC sp_WhatWasBackedUp @DBName = 'MyDB' , @FullBackupsOnly = 1`

***
* __WhatWasRestored.sql__
    * Display the latest DB restores including details of the source backup file.
    * Use optional `@DBName` parameter to narrow down results to specific DB or a subset using wildcards.
    * Use optional `@FullBackupsOnly` parameter with a value of 1 to restrict results to Full Backups.
    * Usage : `EXEC sp_WhatWasRestored @DBName = 'MyDB' , @FullBackupsOnly = 1`

***
* __WhereAreTheBackups.sql__ 
    * Display the location and size of Database backup files for backups taken on the current instance.
    * Use optional `@DBName` parameter to narrow down results to specific DB or a subset using wildcards.
    * Use optional `@FullBackupsOnly` parameter with a value of 1 to restrict results to Full Backups.
    * Usage : `EXEC sp_WhereAreTheBackups @DBName = 'MyDB' , @FullBackupsOnly = 1`

***
* __WhereAreTheFiles.sql__ 
    * Display the location and size of Database Data and Log Files.
    * Use optional `@DBName` parameter to narrow down results to specific DB or a subset using wildcards.
    * Usage : `EXEC sp_WhereAreTheFiles @DBName = 'MyDB'`
    
***