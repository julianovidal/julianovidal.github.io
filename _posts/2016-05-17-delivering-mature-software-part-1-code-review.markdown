---
layout: post
title:  "Delivering mature software: Part 1 - Code review"
date:   2016-05-17 00:00:00 -0300
---

[Steve McConnell](http://www.amazon.com/Steve-McConnell/e/B000APETRK/ref=dp_byline_cont_book_1) tells on his book [Code Complete](http://www.amazon.com/exec/obidos/ASIN/0735619670/codihorr-20) interesting facts about code review. This has caught my attention:

`“… software testing alone has limited effectiveness — the average defect detection rate is only 25 percent for unit testing, 35 percent for function testing, and 45 percent for integration testing. In contrast, the average effectiveness of design and code inspections are 55 and 60 percent.”`

An interesting study brought in the book as well:

`“In a group of 11 programs developed by the same group of people, the first 5 were developed without reviews. The remaining 6 were developed with reviews. After all the programs were released to production, the first 5 had an average of 4.5 errors per 100 lines of code. The 6 that had been inspected had an average of only 0.82 errors per 100. Reviews cut the errors by over 80 percent.”`

Both examples show us how important and how much benefit a simple culture change can improve the quality of the delivered software.

### “Pair programming is nothing more than code review on steroids”
Talking to some friends from college the other day we discussed how we used to code and how we solved the tasks back in the 2k's.

We would gather all in a room at someone’s frat-house and spend all night coding with everybody around talking and discussing how the code was supposed to be built and how to solve the given problem.

At that time we had no idea that what we were doing was Pair-Programming, but in this case usually was not in “pairs” but in groups.

After sometime the person on the keyboard would go eat something or was tired and was going to rest and someone else would take control of the keyboard and continue the work. In the end we couldn’t have bugged code and couldn’t deliver unreadable code becaCode reviews mentor newer engineersuse our grade depends on how the teacher was going to read it.

### Software engineers do not like to test
Seems like a lame excuse but it is a fact! Most of the software engineers do not like to test or worse, never had to test their own code.

There are companies that have entire teams of Quality Assurance (Q.A) to test their engineers code and if they have fulfilled the requirements correctly.

Why don’t we take all these people and put them to code instead? More software will be delivered I think.

### Code reviews mentor newer engineers
A special aspect of agile is that when new members join the team more seasoned engineers mentor the newer members. And code review helps facilitate conversations about the code base. Often, teams have hidden knowledge within the code that surfaces during code review. Newer members, with fresh eyes, discover gnarly, time-plauged areas of the code base that need a new perspective. So, code review also helps ensure new insight is tempered with existing knowledge.

### “We have tight deadlines and code review take time!”
This is the #1 reason given by engineers for not doing code review. In the end what you will see is less code re-written and less bugs on production. This should be reason enough to do code review.

### Pull request before merge
One benefit that we have when we use Github or Bitbucket is the pull request feature. I used this feature for 3 main things:

* We can code review and comment on commits before it is merged
* We can track the merges and rollback if something is broken.
* We can build and run tests after a merge.

### Coding standards
Everybody has his/her code style and most companies have a standard to code. From simple brackets to full class patterns. In this case code review guarantees that everybody will read the same code style.

### Reuse of code
If you work on a big application and is build on top of several other applications or has a lot of dependencies it is really natural that you will end up creating methods that you did not know that were already there to be used. New eyes bring the knowledge that you might need to know that you could have reused code instead of writing new one.

In the end, instead of thinking on how long will take to make a code review, we have to think on how much money we will save preventing bugs on production and preventing bad feedback from the customers.