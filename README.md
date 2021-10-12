# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

TO BE UPLOADED

### Links

- Solution URL: [LINK TO BE ADDED]()
- Live Site URL: [LINK TO BE ADDED]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- BEM Methodology

### What I learned

- [Inner workings of the stacking context](https://stackoverflow.com/questions/54897916/why-cant-an-element-with-a-z-index-value-cover-its-child), z-index has more to it than it seems, a child element can't cover its parent even if set to a higher positive value; one way is to set the parent's z-index to **auto** and the child's z-index to a **negative value**. There are some hacky alternatives described in the link using 3D transformations

- Writing multiple pseudo element selectors from the same element results in these properties cascading. Very useful here to avoid boilerplate code for each card modifier.

```css
.card::before {
  /* Shared properties */
  position: absolute;
  top: -6px;
}

.card--supervisor::before {
  /* Pseudo-element variations for supervisor modifier */
  background-color: var(--color-cyan);
}

.card--karma::before {
  /* Pseudo-element variations for karma modifier */
  background-color: var(--color-yellow);
}
```

### Continued development

I'm a huge culprit in using Flexbox for everything, I specifically picked this challenge to further improve my Grid skills. It's a wonderful tool I haven't been properly using.

### Useful resources

- [Tutorial on Drop Shadows](https://www.freecodecamp.org/news/css-tutorial-drop-shadow/) - Straight forward article on how to apply box shadows.
- [Complete guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - CSS-Tricks never fails.

## Author

- Twitter - [@codingtomato](https://twitter.com/codingtomato)
- Frontend Mentor - [@VeryEvilTomato](https://www.frontendmentor.io/profile/VeryEvilTomato)