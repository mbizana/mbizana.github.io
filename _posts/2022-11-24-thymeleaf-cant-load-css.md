---
layout: post
title:  "Thymeleaf cannot load css"
date:   2022-11-24 16:29 +0000
categories: software development
#author: Zuko Mgwili
---

Recently as part of an effort to ramp up on (Spring)(https://spring.io/projects/spring-boot) in preparation for a new project, I ran into an issue. The issue was: the css was not being applied to a page. I had the following in my [Thymeleaf](https://www.thymeleaf.org/) template:

```
<link rel="stylesheet" th:href="@{/style.css}" />
```

After much googling and trial and error, the solution that worked is the following:

```
<link rel="stylesheet" th:href="@{/css/style.css}" />
```

It turns out that I needed to move the css file to a folder and not have the css file  at the root of the ***static*** folder.