# JavaScript Virtual DOM

## Objectives

1. Explain what a virtual DOM is
2. Describe why a virtual DOM might be useful
3. Describe some of the tradeoffs of using a virtual DOM

## Overview

We want to give students a very high-level look at virtual DOMs in the abstract.
It's totally okay to focus on React, but students should understand that React's
isn't the only virtual DOM implementation in town, and they should also
understand that React is more than simply a virtual DOM (even if that's one of
its core ideas that it happens to execute very well).

It's worth mentioning some of the tradeoffs w/r/t to reconciling virtual and
actual state. Inputs are a bit wonky (but more on that in a later lesson, of
course), and side effects in when rendering can grind an application to a halt.

At the same time, JavaScript is fast while the DOM APIs are slow — this point is
worth emphasizing.

## Resources

- [Why did we build React?](https://facebook.github.io/react/blog/2013/06/05/why-react.html)
- [React (Virtual) DOM Terminology](https://facebook.github.io/react/docs/glossary.html)
