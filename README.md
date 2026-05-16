# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Links

- Solution URL: [https://github.com/Krysmynta/social-links-profile]
- Live Site URL: [https://krysmynta.github.io/social-links-profile/]

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learned that my solution to a previous challenge (blog review card) did not work the way I thought it did, with regard to my use of flex-basis as a means of making the site responsive. Since the parent container (body) of the blog card is a flex container with flex-direction 'column', flex-shrink (which shrinks across the main axis) and flex-basis cannot be used to shrink the card horizontally. A much simpler and more reliable way of making a simple blog card design responsive to smaller screens is setting a width in combination with a max-width of 100%, which is what I did in this challenge. The max-width of 100% allows the card to shrink below its original/default width.

I also learned about the pseudostates :focus and :focus-visible, which enables easy navigation between links using the tab key. :focus-visible ensures that the links get high-lighted only via keyboard (not by mouse klicking). 

Code snippets from my solution:

```css
.profile-card {
  width: 350px;
  max-width: 100%;
}

.social-links:focus-visible {
  outline: 2px solid var(--Green);
  outline-offset: 2px;
}
```

### AI Collaboration

To get to my solution for this challenge I had discussions with GitHub Copilot and later ChatGPT.


## Author

- Frontend Mentor - [@Krysmynta](https://www.frontendmentor.io/profile/Krysmynta)


