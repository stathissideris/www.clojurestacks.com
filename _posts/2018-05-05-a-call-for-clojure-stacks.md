---
layout: post
author: Stathis Sideris
title:  "A call for Clojure stacks"
date:   2018-05-06 22:10:22 +0300
categories: misc
---

People start learning Clojure, get really excited about it (because
it's awesome!) and they decide to make a web app because web apps are
the Hello World of our time. And then they get a bit lost by having
too many options and they are slightly bemused by the lack of an
"official" framework for making this kind of app.

The culture shock seems to be especially pronounced for people coming
from a Ruby on Rails background, persumably because they have to make
decisions about aspects of the stack that have been already settled
years ago in Rails.

The community's responce is always an enthusiastic "do anything you
like!" or "it's
[decomplected](https://www.infoq.com/presentations/Simple-Made-Easy),
it all plays well together, just pick something!". But there is no
denying that the amount of choice is daunting to newcomers --
 sometimes to the point of being completely off-putting. I still
believe the fact that no "official" Clojure web framework has emerged
is a good thing, but there is no denying that we could do more as a
community to lower the barrier of entry.

So, this is a call for Clojure stacks. I'm looking for teams who have
built web apps, frontend apps, mobile apps or anything else, and who
are willing to take a look at their `project.clj` files, their
`build.boot`s or `deps.edn`s and explain the reasoning of the choices
reflected there, along with the rest of the system (the non-Clojure
parts), and also the pros and cons of that particular combination of
choices. Some bricks fit together better that others, and sharing this
knowledge can only help Clojure grow.

Here are some questions that you could use as a template for your
post, or feel free to send a more free form explanation:

- What is your app?

    REST API, ClojureScript frontend, mobile app, desktop app etc.

- What business requirement does it cover?

- When did development start? Is it still going on?

    This is important because a large part of the stack is decided at
    the beginning of the project, and from that point onward central
    libraries are not refactored out very frequently. Also, the
    ecosystem evolves pretty rapidly and the choices you have right
    now are different to what you had a few years ago.

- What's the overall architecture/stack of your system?

    REST? Web sockets? React? Multithreaded? What's your database?
    Message queues? Caching?

- What libraries did you use and why?

    The most important part of the description of the stack. How do
    you do REST? What about routing? How do you handle state in the
    frontend? What do you use for templating (and can a designer
    contribute)? How do you use spec? What do you use for logging
    (local and remote)? How about monitoring? Any special libraries
    for loading your config?

- Are you pleased with your choice of libraries?

    Did you face any problems with any of the libraries? Did you face
    any incompatibility issues between libraries? Did you have to
    write a lot of glue code to get them to work together?

- If there was zero development cost in replacing one of the libraries
  for a better/newer one, what replacement would you make and why?

- Code architecture

    Do you do MVC? How do you separate your code in namespaces?

- What test methodologies do you use? What are your thoughts on your
  experience with it?

    Unit tests, generative testing, simulation testing,
    [transcriptor](https://github.com/cognitect-labs/transcriptor).

- What's in your dev profile and how is it helping you?

    Libraries that improve stack traces, libs for spec error messages,
    anything that helps with the process but it's not part of the
    final artifact.

- Dev tools

    Editors, build tools, dependency resolution tools, lint tools,
    test runners, packaging tools, deployment tools, what's your
    secret mix?

- Infrastructure

    Do you deploy on AWS (EC2, ECS, Fargate, Lambdas) , Google Cloud,
    Azure, Raspberry Pi, your laptop, Docker.

- Final remarks

It's a lot to ask, and not every organization will be OK with sharing
all the details, so share as much as you can. Descriptions of "failed"
stacks may also be useful. Contributions are super-welcome in markdown
by pull request to
[this repo](https://github.com/stathissideris/www.clojurestacks.com).
