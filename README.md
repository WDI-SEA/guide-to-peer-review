# Code Reviews

## What is code review?

Code review is any process where people review code that has already been
written. Generally this is to identify errors or to suggest ways the code could
be improved (refactored).

## Why do code reviews?

Jeff Atwood (co-founder of Stack Exchange, and a smart dude) has written a
[great summary](http://blog.codinghorror.com/code-reviews-just-do-it/) which I
encourage you to read. The short verion? Code review can reduce the number of
errors in our programs dramatically.

At the end of the day, our work and our programs are only as healthy as our overall code base. Without thorough, regular code review further errors, bugs, and overall tech debt can grow. 

In addition we believe that learning to read code critically is an important
part of improving our own code. After all, to improve our own code, we must read
it, looking for ways to improve it.

Additionally, many work environments practice some form of code review, so it's
good to get practice in giving feedback to others now. Even if your future
workplaces don't have a formal code review process, you may find them so helpful
that you implement your own informal practices with your teammates!

## How to Code Review?

At it's core, doing a code review is just reading code and giving feedback.
When reading code, you should be looking for:

* code quality - [STACHE guidelines](stache-guidelines.md), patent pending ;)
* potential bugs

When giving (and recieving) feedback, remember that we're discussing and
commenting on code, not the person who wrote it! Be well intentioned in both your critique and commentary. 

There are a few ways we can actually read the code and give feedback:

### Read The Most Recent Version (Full-Context)

One way is to just read through the most recent version of the codebase. (i.e.
use Github to browse the most recent commit/code). If you do a pull request, you can also give feedback as you're reading to the person or
by leaving comments in the code.

### Read What's Changed (Diff)

Another way is to review just the code that's changed since you last reviewed,
and give feedback on that.

Github will show you the changes between any two branches, commits, etc,
including by time!

To see this view, use a URL like:
https://github.com/<USER>/<REPO>/compare/master@{1day}

This will show the difference between the current master branch (implied), and the
master branch 1 day ago. Make sure to select the appropriate time frame.

### Which Way is Correct?

There is no one correct way to do a code review. What is most important is that you and your teammates take the time to A. check for errors, B. learn from how others solved the problem, C. learn about why you solved the problem the way you did. Peer code reviewing allows us to do all of this. 

Still lost on how to start? [Read this guide here](https://google.github.io/eng-practices/review/reviewer/looking-for.html) from the Google Engineering team on what to look for in a code review. 