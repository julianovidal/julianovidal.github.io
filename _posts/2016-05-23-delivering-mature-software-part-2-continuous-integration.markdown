---
layout: post
title:  "Delivering Mature Software: Part 2 - Continuous Integration"
date:   2016-05-23 00:00:00 -0300
---

Okay, so you have built a small application and you have to test it before it goes into productipend less time debugging and more time adding features, will stop waiting to find out if the code is going to work and will increase the confidence to deploy into production.on. You then write some JUnit tests, goes trough all the happy paths and possible scenarios you can remember to test and then deploy the new package into production. So far, so good.

After some time your application starts to grow, you have other peers in your team, your application start to get broken into minor applications and start to become more distributed since you need everything to be scalable and when you realize it, you have an application with thousands of JUnit tests and hundreds of test cases you have to test before it goes into production.

Then you face 2 possible solutions:

* Build a Quality Assurance team (Q.A Team) and start to wait weeks or even months to deliver a single change request.
* Change the way your team code and create and Continuous Integration environment.
I believe that the second approach has more benefits.

At first, it seems that you will waste a lot of time and money, but when you put all the pieces together and start to track the number of bugs you used to have on production and if is the case the money losses you will reduce, then you see this as a valuable asset to your company.

`“Continuous Integration doesn’t get rid of bugs, but it does make them dramatically easier to find and remove.”`

`- Martin Fowler, Chief Scientist, ThoughtWorks`

### How the process may happen
There are many ways to build a Continuous Integration process. This is just an example.

Developers code into their local repositories or branches. When done, they commit into the repository.

The CI Server monitors every commit into the repository and start a new build when the code is committed.

During the build the CI Server runs the unit tests and if the build does not fail it will start the integration tests.

After the successful build of the integration tests the new version is available to be delivered into production.

If the build fails the team gets an alert message and a report of the failed reason.

Usually the person/team who committed the code is responsible for fixing the code and committing again for a new build. 

![font: https://www.mera.com/services/processes/integration](https://www.mera.com/media/attachments/2016/05/29/continious_integration.jpg)

When introducing these practices the team will start to experience a lot of benefits which includes spend less time debugging and more time adding features, will stop waiting to find out if the code is going to work and will increase the confidence to deploy into production.

