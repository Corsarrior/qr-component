# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![Screenshot](./screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://github.com/Corsarrior/qr-component.git)
- Live Site URL: [Add live site URL here](https://qr-component-challenge.glitch.me/)

## My process

### Built with

- CSS variables
- Flexbox

### What I learned

I was using viewport units to determine the width and height of the card, but on some devices, like the ipad, the relationship between the two dimensions was out of proportion. So I discovered that I can use the calc function and CSS variables to define the height of the component based on its width:

```css
    .qr-card {

      width: var(--width);
      height: calc(var(--width) * 1.55);
      border-radius: 4.5%;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      background-color: hsl(0, 0%, 100%);
      
    }
```

The calc function was also useful for defining the size of fonts based on their containers:

```css
   .text-1 {
      font-weight: 700;
      font-size: calc(var(--width) * 0.07);
      opacity: 0.82;
      flex-grow: 1;
      flex-shrink: 0;
      flex-basis: auto;

    }
```
Finally, the most important learning was the use of Flexbox, which seems easy at first, but is more challenging and complext than I thought.


## Author

- Frontend Mentor - [@Corsarrior](https://www.frontendmentor.io/profile/Corsarrior)
- Twitter - [@JuanQB94](https://www.twitter.com/yourusername)

