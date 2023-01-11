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
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot
![Mobile Version](https://bit.ly/3AngTfg)
![Desktop Version](https://bit.ly/3ct4qPg)

### Links

- Solution URL: [Click here](https://bit.ly/3pOjNEO)
- Live Site URL: [Visit here](https://odagora.github.io/product-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- BEM methodology

### What I learned

Use of CSS Grid responsively without the need of Media Queries
```css
.product-container {
    position: relative;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(375px, 1fr));
}
```
`overflow` property to display correctly an image inside a parent component with a `border-radius`
```css
.product-container {
    overflow: hidden;
}
```
Use of accesibility text for screen readers
```html
<p class="product__price">
  <span class="visually-hidden">Current price:</span>
  $149.99
</p>
```
```css
.visually-hidden:not(:focus):not(:active) {
    clip: rect(0 0 0 0);
    clip-path: inset(50%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap;
    width: 1px;
}
```
### Continued development

- Use of preprocessors like SASS for styling
- Use of CSS Grid in complex layouts
- Use of transformations and animations with CSS

## Author

- Website - [Daniel González](https://odagora.com/)
- Frontend Mentor - [@odagora](https://www.frontendmentor.io/profile/odagora)
- Twitter - [@odagora](https://www.twitter.com/odagora)

## Acknowledgments

The Frontend Platzi courses helped me with the basic concepts of semantic HTML, CSS3 and BEM methodology. Also, I implemented best practices regarding responsive design, performance and accesibility.
