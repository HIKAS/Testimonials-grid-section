# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)

  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)

- [My process](#my-process)

  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

  - [Useful resources](#useful-resources)

- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./design/Web%20capture_15-2-2023_141117_127.0.0.1.jpeg)

![](./design/Web%20capture_15-2-2023_135816_127.0.0.1.jpeg)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

using the CSS grid to implement Responsive Web design

```css
@media (min-width: 600px) {
  .container {
    max-width: 1440px !important;
    margin: 5px;
  }
  .testimonial-section {
    margin: 0;
  }
  .container {
    display: grid;
    grid-template-columns: auto auto auto auto;

    grid-template-rows: auto auto;
    gap: 25px 25px;
  }
  .container > article:nth-child(1) {
    grid-area: 1 / 1 / span 1 / span 2;
  }
  .container > article:nth-child(2) {
    grid-area: 1 / 3 / span 1 / span 1;
  }
  .container > article:nth-child(3) {
    grid-area: 2 / 1 / span 1 / span 1;
  }
  .container > article:nth-child(4) {
    grid-area: 2 / 2 / span 1 / span 2;
  }
  .container > article:nth-child(5) {
    grid-area: 1 / 4 / span 2 / span 1;
  }
}
```

### Useful resources

- [CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - This helped me . I really liked this pattern and will use it going forward.

## Author

- Frontend Mentor - [HIkas](https://www.frontendmentor.io/profile/HIKAS)
