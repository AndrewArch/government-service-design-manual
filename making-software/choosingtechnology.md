---
layout: detailed-guidance
title: Choosing technology
subtitle: How to go about choosing what software tools to use
category: making-software
type: guide
audience:
  primary: developer, tech-arch
status: draft
phases:
  - alpha
  - beta
---
    
# Choosing technology

At different points in your project you'll have to choose one technology
over others. That might be a programming language, database, operating
system or some small tool that helps the development team work more
efficiently.

## Guidance

### You can change your mind

The most important consideration is to work on the assumption that most
technology choices can change, especially during the early stages of
development. On day one of your project you simply won't know enough
about the domain or the user need to select the _right_ technology. 
It's OK to make an educated guess at this stage, as long as everyone
understands that is what is happening. Then find time to challenge the
selection as you learn more about the problem at hand.

Maybe you selected a programming language that you knew would be easier
and quicker to prototype in for the early stages of the project, and then
moved to another one that was easier to work in large teams with for the
final product. Or maybe you started out with an open source product to
allow you to get started quickly, before going on to buy a commercial
product which provided some required feature.

### Start with capabilities, not implementations

It's very easy to immediately jump to a specific product when making
technology choices. This tends to be based either on past experience or
on fashion, so deciding up front that you will use Oracle or that
MongoDB is what you require. Try and take a step back and think about
the capabilities of the technology you're after. Are you looking for a
relational database? Or a document database? A key/value store? Or maybe
a graph database? Argue first about the capabilities, rather than any
specific implementation.

### Cost

With the growth of open source many technology products; databases,
operating systems, programming languages, development tools, etc. are
freely available. But a large market still exists for commercial
software products. When choosing technology make sure you do consider
the total cost, as well as any upfront fees. Try and take into
consideration costs for things like staff, support and productivity.

### Consider people

Try and involve the whole team in technology choices. That doesn't mean
no-one owns the decision making but that you want the development team
to buy in to the technology choices made. Technology preferences
vary, and technology choice can divide opinion. All things being equal,
picking technologies that developers and operations staff like will
likely result in improved productivity.

### Lock-in

Technology lock-in happens when previous decisions regarding technology
limit future decisions, possibility so that only one real choice exists.

For example, if you select a database that only runs on one operating
system you have no choice about the operating system you will use. If the
costs of that operating system jump you have no simple way of reducing
that cost quickly or cheaply.

Over time, and after many decisions, you can find yourself in a
situation where all your technology decisions are tightly coupled and
you are locked-in to one vendor or one way of doing things. This can
have unforseen financial costs (for example an overnight cost increase)
but can also limit how quickly you can iterate on your product in the
future, for instance if the ideal technology choice isn't compatible
with your current vendor or technology.

## Why we do this

Choosing technology is important, but it's probably not quite as
important as you think. What is important are the users of that
technology and being able to deliver quality at a sustainable pace and
suitable cost. When making technology choices, and importantly as you
develop your product and constantly reassess your selections, try and
make decisions that:

* Maximise developer productivity
* Minimise total cost of ownership
* Avoid lock-in

## Further reading

* Open Source Considerations (link to guide)
