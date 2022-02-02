# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./images/solution.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- BEM Methodology
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I think my major learning of this project was without a doubt how to overlay the icon, it took me a few more hours than I thought it would, triying on my own before I searched a similar solution on the web.

```html
<figure class="card__figure">
  <img src="./images/image-equilibrium.jpg" alt="nft" class="card__image">
  <div class="overlay">
    <a href="#" class="overlay__icon"></a>
  </div>
</figure>
```
```css
.card__figure{
    margin: 0;
    position: relative;
    padding: 25px 25px 16px;
}

.card__image{
    max-width: 100%;
    border-radius: 10px;
}

.overlay{
    margin: 25px 25px 16px;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 300px;
    width: 300px;
    opacity: 0;
    transition: 0.3 ease;
    background-color: hsla(178, 100%, 50%, 0.5);
    border-radius: 10px;
}

.overlay:hover{
    opacity: 1;
    cursor: pointer;
}

.overlay__icon{
    position: absolute;
    top: 50%;
    left: 50%;
    height: 50px;
    transform: translate(-50%, -50%);
}
```

### Useful resources

- [Overlay Icon](https://www.w3schools.com/howto/howto_css_image_overlay_icon.asp) - This helped me to learn how to overlay an icon with hover

