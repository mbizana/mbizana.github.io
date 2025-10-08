---
layout: post
title:  "Missing xcrun"
date:   2022-11-19 16:20 +0000
categories: software development
#author: Zuko Mgwili
---

I had just pulled a Ruby on rails project from Github and then proceeded to execute the following command:

```
bundle install
```

I then encountered the following error

```
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun
at: /Library/Developer/CommandLineTools/usr/bin/xcrun

An error occurred while installing bootsnap (1.14.0), and Bundler cannot continue.

In Gemfile:
  bootsnap

```

To resolve the issue, I ran the following command

```
xcode-select --install
```


