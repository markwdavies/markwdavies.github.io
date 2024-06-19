---
title: No More Lucky Numbers
layout: post
tags: news misc sql
author: mwd
---

# {{ page.title }}

After a long period of silence, an update. I have removeded the stored procedure sp_WhatAreMyLuckyNumbers stored proc out of the public repo.
A random number generator is probably a little too frivolous in this context.
It could also be massively inefficient when the parameters were tweaked to select more unique numbers from a wider range than the default six numbers between 1 and 49.