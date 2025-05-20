# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK).
## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./public/images/project%20screenshot.png)

### Links

- [Solution LINK](https://your-solution-url.com)
- [Live Site LINK](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- Sass/SCSS - modular, variables, mixins
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Vite](https://vite.dev/) - Build tools

### What I learned

I finally got to use CSS Grid for real in this project—and wow, it's powerful! I’m still wrapping my head around everything it can do, but even with what I know so far, it made laying things out so much easier.

While building the layout, I experimented with both:
- grid-template-columns / grid-template-rows
- grid-template-areas

Both worked really well, but I ended up using the latter one:
```scss
.feature__nav {
    display: grid;
    gap: $space-lg;

    @media (min-width: 768px) {
        grid-template-areas: 
        "top top"
        "mid1 mid2"
        "bottom bottom";
    }
    @media (min-width: 1440px) {
        grid-template-areas: 
        "left mid1 right"
        "left mid2 right";
    }
}
```

### Continued development

Flexbox and CSS Grid are definitely things I want to keep working on. They’re super powerful for building responsive layouts, and I’m really looking forward to getting more confident with them and learning all the cool stuff they can do.

I also want to keep practicing being more mindful while I code—like really thinking through what each change does, whether it’s affecting the layout, the logic, or how things behave in the browser. And along with that, I want to get better at writing clear commit messages that actually reflect what I did.