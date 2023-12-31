# Frontend Mentor - Interactive pricing component solution

This is a solution to the [Interactive pricing component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-pricing-component-t0m8PIyY8). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Use the slider and toggle to see prices for different page view numbers

### Screenshot

![Dekstop](/Screenshot/Desktop.png)
![Tablet](/Screenshot/Tablet.png)
![Mobile](/Screenshot/Mobile.png)

### Links

- Solution URL: [Github](https://github.com/Aayush895/Interactive-Pricing-Component)
- Live Site URL: [Netlify](https://interactive-slider-component.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Through this project, I learned how to create a basic interactive slider that changes the value of the content every time the value of the slider is changed. I also learned how to create a custom toggle button through basic HTML and CSS.

The code for interactive slider is mentioned below: 

```JS
function changeValue(e) {
  if(e.target.value == 8) {
    pageViews.innerText = '10K'
    requiredAmount.innerHTML = '$8.00 <span>/month</span>'
  }

  if (e.target.value == 12) {
    pageViews.innerText = '50K'
    requiredAmount.innerHTML = '$12.00 <span>/month</span>'
  }

  if (e.target.value == 16) {
    pageViews.innerText = '100K'
    requiredAmount.innerHTML = '$16.00 <span>/month</span>'
  }

  if (e.target.value == 24) {
    pageViews.innerText = '500K'
    requiredAmount.innerHTML = '$24.00 <span>/month</span>'
  }

  if (e.target.value == 36) {
    pageViews.innerText = '1M'
    requiredAmount.innerHTML = '$36.00 <span>/month</span>'
  }
}

slider.addEventListener('input', changeValue)
```

### Continued development

Through this project, I learned about how to build an interactive slider component, which is something I didn't know how to create before. In the future, I want to create a similar component that will be more refined and better than this one.

### Useful resources

- [Interactive Slider](https://stackoverflow.com/questions/66021399/using-a-range-slider-to-continuously-change-an-input-value-even-when-the-mouse-i) - This stack overflow article helped me get an idea of how I can build an interactive slider.

- [Toggle Button](https://www.youtube.com/watch?v=uCjDIMADK0w) - This YouTube video played a great role in helping me build my own custom toggle button.

## Author

- Frontend Mentor - [@Aayush895](https://www.frontendmentor.io/profile/Aayush895)
- Twitter - [@JhaAayush895](https://www.twitter.com/JhaAayush895)

## Acknowledgments

I would like to thank the entire frontend-mentor team for providing such interesting challenges to test and improve my skills in the domain of frontend web development.