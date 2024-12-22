# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### Screenshot
Desktop version:\
\
![image](https://github.com/user-attachments/assets/6ae749e0-8c5a-4760-8bc2-89b34b0aad00)

Mobile version:\
\
![image](https://github.com/user-attachments/assets/581fbf8c-d570-4394-a94d-47129df6128d)


### Links

- Solution URL: https://holl4444.github.io/qrCode/

## My process
I went into this project having predominantly used Flexbox to build webpages, I used this as an opportunity to learn a few techniques for non-responsive models.A fair amount of the time went to reading up a little on Figma, as the designs were included free with this challenge, providing a fantastic chance to check it out.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Figma

### What I learned

How designs are laid out in Figma: in a similar way to DevTools. Using Figma provided a real moment of clarity for me, having a better overview from the start of the project, and beginning to make classes for different styles rather than applying styles as needed to element's classes. Much tidier!

```css
.slate-500 {
  color: #68778d;
  font-size: 0.93rem;
  letter-spacing: 2.5rem;
}
```
It was also interesting to play around with responsive property values within the non-responsive framework, I wasn't even sure that was possible! After watching a few videos I understood that I should divide by 16 to find the rem/em version of pixels (as long as the default font-size hasn't been altered).

What a relief to find that using ``` position: absolute ```, which I had found very daunting (and had probably been trying to avoid to some degree!) was not so bad! I was stymied for a little while trying to work out how to make my "attribution" ```<div>``` line up with the main content of this project. Ultimately it led meto explore anchors, which I can see being very useful in some conditions.

``` css
.anchor {
  anchor-name: --anchor;
}

.attribution {
  width: fit-content;
  position-anchor: --anchor;
  position: absolute;
  position-area: end center;
  /* top: anchor(bottom); */
  left: anchor(left);
  margin-top: 10vh;
}
```
The final challenge for me, was how to implement changes for users on a mobile device. In the style guide I saw that the mobile design was tailored to a width of 375px so I started there, but made sure to play around with some other mobile device dimensions in the device toolbar in DevTools. ![image](https://github.com/user-attachments/assets/d02a0178-c4cd-4d91-96bb-d1b76de46907)

### Continued development

I came across the phrase 'mobile-first design' during the last stage of this project! In future projects I'll try to start with the mobile design and work upwards in size. Definitely some reading to be done both with the concept of mobile first design but also with using @media queries.

Putting in some more time with positions other than flex and grid would probably be really beneficial too.


### Useful resources

Here's a link to the video that helped me understand why to use responsive values and how to calculate them.
https://www.youtube.com/watch?v=mh39YXytfC0

## Author

- Frontend Mentor - [@Holl4444](https://www.frontendmentor.io/profile/Holl4444)
