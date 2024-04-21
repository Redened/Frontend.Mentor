# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

-   [Overview](#overview)
    -   [The challenge](#the-challenge)
    -   [Screenshot](#screenshot)
    -   [Links](#links)
-   [My process](#my-process)
    -   [Built with](#built-with)
    -   [What I learned](#what-i-learned)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](Desktop.png)

### Links

-   Solution URL: [https://www.frontendmentor.io/solutions/recipe-page-html-scss-v5P20SdLiz](https://www.frontendmentor.io/solutions/recipe-page-html-scss-v5P20SdLiz)
-   Live Site URL: [https://redened.github.io/Frontendmentor-Project04/src/](https://redened.github.io/Frontendmentor-Project04/src/)

## My process

### Built with

-   Semantic HTML5 markup
-   SCSS
-   Flexbox
-   Mobile-first workflow

### What I learned

Custom Disc or ::marker for Unordered lists using CSS li:before selector.

```css
ul {
    list-style: none;
}

li {
    display: flex;
    align-items: center;
}

li:before {
    content: "•";
    font-size: 15pt;
    margin-right: 2.5rem;
    color: hsl(14, 45%, 36%);
}
```


Custom Number or ::marker for Ordered lists using CSS li:before selector and CSS counter property.

```css
ol {
    list-style: none;
    counter-reset: ordered-list-item;
}

li {
    display: flex;
    align-items: first baseline;
    counter-increment: ordered-list-item;
}

&:before {
    content: counter(ordered-list-item) ".";
    font-weight: 700;
    margin-right: 2rem;
    color: hsl(14, 45%, 36%);
}
```
