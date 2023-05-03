# Programming Principles

Every programmer benefits from understanding programming principles and design
patterns. This overview is a reference for myself, and maybe it is of help to
you during design, discussion, or review. The list is incomplete, and sometimes
trade-offs need to be made between conflicting principles. However, higher
ranked principles usually beat lower ranked ones.

The list was inspired by <!-- markdown-link-check-disable-next-line -->
[The Principles of Good Programming](https://www.artima.com/weblogs/viewpost.jsp?thread=331531)
(down?
[Google's cache](https://webcache.googleusercontent.com/search?q=cache:KU51T8hZ-0kJ:https://www.artima.com/weblogs/viewpost.jsp%3Fthread%3D331531+&cd=1&hl=en&ct=clnk&gl=nl&client=pub-3911176865765226)).
I've added a bit more reasoning, details, and links to further resources.
[Let me know](https://github.com/webpro/programming-principles/issues) if you
have any feedback or suggestions for improvement!

## Contents

### Generic

- [KISS](#kiss)
- [YAGNI](#yagni)
- [Do The Simplest Thing That Could Possibly Work](#do-the-simplest-thing-that-could-possibly-work)
- [Separation of Concerns](#separation-of-concerns)
- [Keep things DRY](#keep-things-dry)
- [Code For The Maintainer](#code-for-the-maintainer)
- [Avoid Premature Optimization](#avoid-premature-optimization)
- [Boy-Scout Rule](#boy-scout-rule)

### Relationships between modules, classes, components, entities

- [Connascence](#connascence)
- [Minimise Coupling](#minimise-coupling)
- [Law of Demeter](#law-of-demeter)
- [Composition Over Inheritance](#composition-over-inheritance)
- [Orthogonality](#orthogonality)
- [Robustness Principle](#robustness-principle)
- [Inversion of Control](#inversion-of-control)

### Modules, classes, components, entities

- [Maximise Cohesion](#maximise-cohesion)
- [Liskov Substitution Principle](#liskov-substitution-principle)
- [Open/Closed Principle](#openclosed-principle)
- [Single Responsibility Principle](#single-responsibility-principle)
- [Hide Implementation Details](#hide-implementation-details)
- [Curly's Law](#curlys-law)
- [Encapsulate What Changes](#encapsulate-what-changes)
- [Interface Segregation Principle](#interface-segregation-principle)
- [Command Query Separation](#command-query-separation)
- [SOLID](#solid)

### Test

- [FIRST principles of testing](#first-principles-of-testing)
- [Arrange, Act, Assert](#arrange-act-assert)

## KISS

**Keep It Simple, Stupid**: most systems work best if they are kept simple
rather than made complex.

Why

- Less code takes less time to write, has less bugs, and is easier to modify.
- Simplicity is the ultimate sophistication.
- It seems that perfection is reached not when there is nothing left to add, but
  when there is nothing left to take away.

Resources

- [Keep It Simple Stupid (KISS) (principles-wiki.net)](http://principles-wiki.net/principles:keep_it_simple_stupid)

## YAGNI

**You Aren't Gonna Need It**: don't implement something until it is necessary.

Why

- Any work that's only used for a feature that's needed tomorrow, means losing
  effort from features that need to be done for the current iteration.
- It leads to code bloat; the software becomes larger and more complicated.

How

- Always implement things when you actually need them, never when you just

