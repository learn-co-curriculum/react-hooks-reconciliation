# JavaScript Virtual DOM

## Objectives

1. Explain what a virtual DOM is
2. Describe why a virtual DOM might be useful
3. Describe some of the tradeoffs of using a virtual DOM

## What's a virtual DOM?
![React VR?](https://media.giphy.com/media/3o7qDL7l1IZAQvxvj2/giphy.gif)

By now, you should already know what the DOM is: a programmatic representation of the document we see in the browser.
So, what's all this virtual DOM ruckus about? Well, it turns out that our good 'ol friend DOM is slow — terribly slow. He
makes a granny using a walker look like Usain Bolt.

Virtual DOM is a technique employed by several front-end libraries and frameworks, most notably React. In a nutshell,
virtual DOM builds a _virtual_ representation of what our document should look like. When we're ready to render things
to the screen, the virtual DOM will take a look at the existing DOM and change only what needs to be changed (in more
technical terms, it's diffing and re-rendering the changes).

The performance gains here are not to be underestimated, due to the way the virtual DOM works. Virtual DOM is created by
a bunch of super smart people using extremely efficient algorithms. Most virtual DOMs also batch their updates to the
DOM, ensuring that the _real_ DOM gets modified as little as possible. The point is: it's best to touch and change the
DOM as little as possible, and when we do, we do it with surgical precision. Think of virtual DOM as our personal DOM
surgeon!

## So why use it?
The above section should have already given you a good idea of when a virtual DOM is useful. It's a particularly great
choice when we're building apps where changes in the interface happen a _lot_. By reducing the load on the real DOM, we
can make our apps behave much more fluently and in line with what a user expects from software nowadays.

In virtual DOM, we can just say 'okay, our document should look like _this_' — and the virtual DOM will do the heavy
lifting for us (i.e. diffing the changes and applying them). This means that we don't need to write imperative code to
update every tiny bit of our application, we just declare what the end result should look like, and the virtual DOM will
do the rest!

These abstractions also paved the road for non-DOM implementations for virtual DOM, for example React Native. In this
case, it's easier to think of DOM as a generic document, rather than the thing we see in our web browser.

## What's the catch?
Even though virtual DOM is very performant and used in several high-profile libraries and frameworks, it's important to
remember that it's still a _really_ clever workaround. There are other solutions in the works (like Shadow DOM) by
browser vendors to make the DOM faster, but for right now, virtual DOM seems to be our best bet.

## Resources
- [Why did we build React?](https://facebook.github.io/react/blog/2013/06/05/why-react.html)
- [The difference between Virtual DOM and DOM](http://reactkungfu.com/2015/10/the-difference-between-virtual-dom-and-dom/)
- [React (Virtual) DOM Terminology](https://facebook.github.io/react/docs/glossary.html)
