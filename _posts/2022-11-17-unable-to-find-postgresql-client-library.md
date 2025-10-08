---
layout: post
title:  "Unable to find PostgreSQL client library, MacOS 13.0.1"
date:   2022-11-17 11:52:00 +0000
categories: software development
#author: Zuko Mgwili
---

Several times when creating a rails application, I have come across this error, "Unable to find PostgreSQL". The most recent case was when I was creating a rails 7.0.4 application with database option set to 
***postgresql***

```
rails new avongers --database=postgresql
```

The creation process fails with the following message

```
 Unable to find PostgreSQL client library
```

Do the following:

```
brew install libpq
brew link --force libpq
```

Rails should now be able to locate the PostgreSQL client library