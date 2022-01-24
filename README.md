# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Testimonials grid section solution](#frontend-mentor---testimonials-grid-section-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [https://github.com/KrzysztofGrudzien/frontend-mentor-testimonials-grid-section](https://github.com/KrzysztofGrudzien/frontend-mentor-testimonials-grid-section)
- Live Site URL: [https://krzysztofgrudzien.github.io/frontend-mentor-testimonials-grid-section/](https://krzysztofgrudzien.github.io/frontend-mentor-testimonials-grid-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

How to use CSS Grid with Flexbox and Custom CSS Properties with BEM Methodology.


```html
<article class="card card--gray">
    <div class="card__header">
        <img src="./images/image-jonathan.jpg" alt="user image" class="card__img" />
        <div class="card__divider">
            <p class="card__name">Jonathan Walters</p>
            <p class="card__verified">Verified Graduate</p>
        </div>
    </div>
    <h2 class="card__title">The team was very supportive and kept me motivated</h2>
    <p class="card__description">
        “ I started as a total newbie with virtually no coding skills. I now work as a mobile engineer
        for a big company. This was one of the best investments I’ve made in myself. ”
    </p>
</article>
<article class="card card--white card--white-one">
    <div class="card__header">
        <img src="./images/image-jeanette.jpg" alt="user image" class="card__img" />
        <div class="card__divider">
            <p class="card__name">Jeanette Harmon</p>
            <p class="card__verified">Verified Graduate</p>
        </div>
    </div>
    <h2 class="card__title">An overall wonderful and rewarding experience</h2>
    <p class="card__description">
        “ Thank you for the wonderful experience! I now have a job I really enjoy, and make a good
        living while doing something I love. ”
    </p>
</article>

```
```css
.card--white {
    background-color: var(--color-white);
    box-shadow: 40px 60px 50px hsl(217, 19%, 35%, 24.75%);
    color: var(--color-gray-dark);
}

/* ------- DESKTOP ------- */

@media screen and (min-width: 1440px) {
    .cards {
        grid-template-columns: 1fr 1fr 255px 255px;
        grid-template-rows: 290px 266px;
        gap: 2rem;
        height: 572px;
        margin: 0 auto;
        width: 1110px;
    }

    .card {
        margin: 0;
    }

    .card--violet {
        background-position: top right 5rem;
        grid-row-start: 1;
        grid-row-end: 2;
        grid-column-start: 1;
        grid-column-end: 3;
    }
```

## Author

- Website - [In progress]
- Frontend Mentor - [@KrzysztofGrudzien](https://www.frontendmentor.io/profile/KrzysztofGrudzien)
- E-mail - krzysztof.grudzien.fed@gmail.com

