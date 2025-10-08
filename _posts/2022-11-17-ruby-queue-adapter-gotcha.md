---
layout: post
title:  "Ruby queue adapter gotcha"
date:   2022-11-17 10:54:00 +0000
categories: software development
#author: Zuko Mgwili
---

When configuring the queue adapter in Rails 7.0.4 in application.rb file, the value you assign must be a symbol and not a string. I made the mistake of doing the later and I could not get **Resque** to work.

**From:**
```
    config.active_job.queue_adapter = 'resque'
```
**To:**
```
    config.active_job.queue_adapter = :resque
```
