# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./images/screenshot.jpg)

### Links

- Solution URL: [Code Repo](#)
- Live Site URL: [Live site](#)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Bootstrap
- Media queries

### What I learned

I learnt how to switch images on screen resize using the picture tag and media query.

```html
<picture>
  <source
    media="(max-width: 767px)"
    srcset="./images/image-product-mobile.jpg"
  />
  <source
    media="(min-width: 768px)"
    srcset="./images/image-product-desktop.jpg"
  />
  <img
    src="./images/image-product-desktop.jpg"
    class="img-fluid"
    alt="Gabrielle Essence Eau De Parfum A floral"
  />
</picture>
```

```css
@media (max-width: 767px) {
  img {
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    border-bottom-left-radius: 0px !important;
  }
}
@media (min-width: 767px) {
  img {
    border-top-left-radius: 5px;
    border-top-right-radius: 0px;
    border-bottom-left-radius: 5px !important;
  }
}
```

### Useful resources

- [Example resource 1](https://stackoverflow.com/questions/30460681/changing-image-src-depending-on-screen-size) - This article helped me learn how to switch image using media query and picture tags.

## Author

- Github - [jgeev](https://github.com/jgeev)
- Frontend Mentor - [@jgeev](https://www.frontendmentor.io/profile/jgeev)

## Acknowledgments

It was a good UI design challenge. Thank you Frontend Mentor
