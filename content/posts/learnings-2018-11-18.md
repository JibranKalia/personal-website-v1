+++
date = "2018-11-18"
title = "What I learned today: SCSS Ampersands"
slug = "scss-ampersands" 
tags = ["scss"]
categories = ["what I learned today"]
+++

#### Introduction

I am starting a new mini blog concept. I like most software developers learn a lot of small little technical details on a daily basis. That is probably even more true for me because I am still very early in my career. These mini posts are my attempt to record the *aha* moments and the fun tidbits I learn in my journey to becoming a senior software engineer.

##### Ampersand in SCSS

One of the many reasons I love working at Scalefactor so much is that I get to work extensively both in the front-end and the back-end. That being said at the moment, the back-end is my stronger suit. That is why you might see a lot more front-end related posts here as I try to level up in that area. Going back to SCSS. Here is something small I learnt today. Borrowing the explanation below from [CSS-Tricks](https://css-tricks.com/the-sass-ampersand/). 

Here is a simple nesting example that works in SCSS :
 
```css
.parent {
  .child {}
}
```
Which is compiled to in css:

```css
.parent .child {}
```

What about when we use an `&`

```css
.first-parent {
  &.second-parent {}
}
```
Which is compiled to in css:

```css
.first-parent.second-parent {}
```

The difference between the two is that in the second example we are selecting an element that has **both** classes: `first-parent` and `second parent`.


I like to think of `&` as copying the parent selector and pasting it next to the child selector. This gets interesting when used along with [BEM CSS Methodology— Block Element Modifier](http://getbem.com/introduction/). More on that later.

There are a lot more uses of `&` in SCSS. This article in [CSS-Tricks](https://css-tricks.com/the-sass-ampersand/) does an amazing job explaining everything. 

Thank You for reading!