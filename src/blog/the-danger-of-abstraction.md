---
path: /blog/abstractions
date: 2020-03-11T14:15:28.133Z
title: The Danger of Abstraction
tags: Blog
---
Today in history: yet another JS framework is released.

<https://github.com/redwoodjs/redwood>

Prisma! Graphql! React! Yada Yada! Buzzwords! We are building frameworks on top of frameworks. Every time a new one is released, I suffer a bit from what I like to call abstraction creep.

Abstraction creep is the sense that all of these frameworks are so highly opinionated and providing such strong layers of abstraction over the actual details, that by learning just these frameworks we as developers are learning "how to use redwood" as opposed to how to actually do software engineering. Abstraction is all fine and dandy when your project is within the scope of what the abstraction layer was designed to encompass, but the danger, and what causes the abstraction creep so strongly in me, is when a project's requirements fall outside of the abstraction layer. What then is a developer expected to do? Having spent so much time learning specifics defined by this highly opinionated framework, it can be hard to jump outside of the bubble and actually understand what needs to be done. Herein lies the danger of abstraction -- it shields us from a complete understanding in favor of simplicity.

This is not to say abstraction in \_bad\_ per say, but I think its worth considering.\
\
Update:

After spending some time with redwood, I wanted to comment on some notable abstraction examples that have puzzled me already.

1. As a novice to graphql, I am immediately confused how graphql is able to fetch data from the sql database. Is it running sql statements behind the scenes? Who knows! Redwood abstracts this entirely away from the developer, which is great, but I can't help but get hit by abstraction creep. I want to know! It simply feels incomplete to let redwood work its magic while I just plug away happily creating an initial schema and writing graphql queries. I imagine a feature like this is nice after you have a complete understanding of how graphql works, perhaps this avoid the redundancy of writing replicable code, but as a beginner, these are the things I want to know.