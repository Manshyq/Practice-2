# Frontend Mentor - Social media dashboard with theme switcher solution

This is a solution to the [Social media dashboard with theme switcher challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-media-dashboard-with-theme-switcher-6oY8ozp_H) made by Abubakirova Manshuk and Nuranov Atazhan from IT1-2016

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

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Toggle color theme to their preference

### Screenshot

![Dark mode](https://github.com/Manshyq/Practice-2/blob/main/screenshots/final%20dark%20mode.png)
![Light mode](https://github.com/Manshyq/Practice-2/blob/main/screenshots/final%20light%20mode.png)
!["Withous basic CSS"](https://github.com/Manshyq/Practice-2/blob/main/screenshots/without%20basic%20css.png)
![Without JS and how the hover looks](https://github.com/Manshyq/Practice-2/blob/main/screenshots/without%20js%20%2B%20hover.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [React](https://reactjs.org/) - JS library
- [Next.js](https://nextjs.org/) - React framework
- [Styled Components](https://styled-components.com/) - For styles


### What I learned



```html
 <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">

<section class="mode-dark-light">
        Dark Mode
        <div class="mode"><div class="mode__selector"></div></div>
      </section>
```
```css
.card-over {
    background: #252B43;
    transition: .3s;
}

.card-foll:hover {
    background: #333A56;
}
```
```js
function changeMode() {
    if (themeDark) {
        theme.href = 'practice2_light.css';
        modeSelector.classList.add('mode--right');
    }
    else {
        theme.href = 'practice2_dark.css'
        modeSelector.classList.remove('mode--right');
    }
    saveThemeLocalStorage(theme.href);
    themeDark = !themeDark;
}
}
```



### Continued development

We would like to learn more about changing themes of the webpage such as dark and light mode, but with combining it with accessibility, because we have to know what colors it would be better to use in different modes.

### Useful resources

- [Example resource 1](https://stackoverflow.com/questions/8796107/how-to-make-changeable-themes-using-css-and-javascript) - This helped us to learn how to build CSS and JS codes for changing themes.
- [Example resource 2](https://levelup.gitconnected.com/why-dark-mode-causes-more-accessibility-issues-than-it-solves-d2f8359bb46a) - This helped us learn more about the dark and light modes.

## Author

- Website - (https://manshyq.github.io/Practice-2/)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/manshyq)


## Acknowledgments
Before working on projects like this it is really important to understand that changigng modes function is used to help people with using devices and not only for decoration. Also it is important to use different CSS files for different modes.
