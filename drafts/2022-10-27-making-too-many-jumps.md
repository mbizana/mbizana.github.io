13 file code changes later, uncommitted, I am finding myself having to rollback. Even though I have had every intention of strictly making small incremental steps I find myself, over and over making this big jumps. I have intended to always have a working software system, but this is not happening, my software is in a broken state, the application is not running, how did I get here, what can I do to prevent this from happening in the future.

Also on the question of where to start when doing TDD. This is still one of the most perplexing and sometimes frustating things about the process. I've second guessed myself several times. Should I do the inside in approach, inside-out, okay...where should i start is still not answered. what should be my first test. I've settled on testing the flow of a game from start to finish. Even, with this, I'm still unease about this because I am creating test doubles for what I consider not to be central to what I am testing. Then I forget to provide the actual implementation and the application crashes. What should I do here? Have a failing test until all required parts components are implement..maybe?

Another temptation, looking too far into the future. I'm thinking about how different interfaces my interact with the core game logic, then again I end up writing too much logic without accompanying tests.

Back to my 13 files with uncommitted changes. I have made the decision to rollback. I'm going to try my level best to go back to the fundamentals.

One of the things I am committing to is a commit for any atomic change to the codebase. Maybe atomic is the wrong word, a commit for any change addresses one issue. For example, correcting formatting issues raised by a linter, that should result in one commit.

Another commitment, I am making with myself is to always have working software. At any given point in time. I want to be able to run the software. No broken software

I have just attempted to run the software and discovered that there is a missing implement. I should have had tests that fail because of missing implementation because my current suite of tests is green but I still do'nt have working software. I again this is a sign that I made too many big jumps.

I have decided to rollback to the point where I had working software.

I have rolled back to the point where the software is working and the tests are green. There is however a bug that I have identified

What this process has shown is that I need to get back to doing daily code tdd katas. I have let my skills and critical thinking around this lapse and it's time to get back on that horse.