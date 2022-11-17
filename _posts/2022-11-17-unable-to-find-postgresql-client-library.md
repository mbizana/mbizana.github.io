---
layout: post
title:  "Unable to find PostgreSQL client library, MacOS 13.0.1"
date:   2022-11-17 11:52:00 +0000
categories: software development
author: Zuko Mgwili
---

You are creating a rails 7.0.4 project with the database option set to **postgresql** e.g.
```
rails new avongers --database=postgresql
```
The creatiion process fails with the following message
```
 Unable to find PostgreSQL client library
```
Do the following:
```
brew install libpq
brew link --force libpq
```

Rails should now be able to locate the PostgreSQL client library