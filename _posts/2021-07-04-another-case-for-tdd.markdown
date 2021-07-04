---
layout: post
title:  "Another case for TDD"
date:   2021-07-04 09:45:00 +0200
categories: software development
author: Zuko Mgwili
---
I would like to believe that most people in software engineering are fully convinced of the merits of test driven development, but for the very few holdouts out there, maybe this little anecdote from an experience I had will persuade you to at least explore the practice.
<!--more-->
Recently I had a colleague ask me about a section of code that at the time looking at it, it did not make any sense as to why it was there, it seemed redundant. It is an area of the code-base I had not looked at in a while and so my mind was slow in understanding why this seemingly unnecessary code existed. I knew the code had a suite of automated tests that cover the area in question and so I proceeded with reading the tests. Lo and behold! Line 206 of the test suite file was a test describing clearly the purpose of the perplexing code.

A number of things could have happened had we not had any automated tests. We could have fired up the software and then manually debug it to try to figure out what the code is doing. Even worse we could have deleted a supposedly redundant piece of code which would break critical functionality. We did not have to do any of those things thanks to automated tests.
