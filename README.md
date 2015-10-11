# git.rb

## Implementing Git with Ruby

[Git](https://git-scm.com/) is an awesome tool for distributed, collaborative workflows, helping thousands teams build better software everyday.  It's also pretty useful as a version control system for solo work too.  And not just for programming but writing as well - I've been using it to help write my [PhD thesis](https://github.com/davekinkead/thesis) for the last few years.  There is one little problem with it however - git has a freak'n gnarly learning curve that makes understanding it largely inaccessible to Joe Writer or even Jill Developer.

The problem, in my mind at least, is that the way git is typically introduced and explained is too detached from its underlying data model.  Most people think of git as a version control system - probably because that's what the website says and its commands like `commit`, `branch`, and `merge` imply.  

But git is so much more than that.

Learning the fundamentals of anything is critical to understanding it but I found git particularly hard because the most common commands - the porcelain - hide the true nature of what's really going on - the plumbing.  Turns out, git is actually quite scary for many people - seeing your working directory and days of effort disappear before your eyes is never a pleasant feeling.  It all became clearer for me however when I rolled my selves up and got down and dirty in git's data model and tried to commit, branch, and merge manually.

So with that in mind, I thought it might be fun, interesting, and useful even, to dive into the sewers of git's plumbing and re-implement it with ruby, step by step. Just for shits and giggles.  

And to simultaneously scratch another [#becausewhynot](https://twitter.com/hashtag/becausewhynot) itch, I'll be using a library I've written for [literate programming in ruby - Ristretto](https://github.com/davekinkead/ristretto).  This means this project will be split into different lessons that can be transpile into executable ruby file.