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
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

I mostly used flex box to align the items within my the card. I used Psuedo Elements to take care of hover states.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


### What I learned

I garnerd some great knowledge of CSS Flexbox. I also learned a ton about psuedo elements - mainly *::after*

To see how you can add code snippets, see below:

#nftImageContainer {
    cursor: pointer;
    position: relative;
}

#nftImage {
    border-radius: 25px;
    margin-left: auto;
    margin-right: auto;
    max-width:100%;
    max-height:100%;
    position: relative;
    cursor: pointer;
}

#nftImageContainer::after {
    content: "";
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    opacity: 0;
    top: 0;
    left: 0;
    background-color: var(--cyan);
    background-image: url(images/icon-view.svg);
    background-repeat: no-repeat;
    background-position: center;
}

#nftImageContainer:hover {
    opacity: 0.7;
}

#nftImageContainer:hover::after {
    opacity: 0.9;
}


### Continued development

I would live to learn and implement CSS Grid alot more within my projects. It seems easier. I also would like to start using pseudo elements alot more.

## Author

- Twitter - [@SourceCodeDad](https://twitter.com/SourceCodeDad)


## Acknowledgments

Thank you Grace!!!
