# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- See hover states for interactive elements

### Screenshot

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

construction de la structure puis styling des box une par une.
L'ombre sur le bouton, l'ajustement de l'image sont les tâches qui m'ont pris le plus de temps

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- sass

### What I learned

Pour flexbox:

- main axis == justify-content, quelque soit le flex orientation

- cross axis = align-items, quelque soit le flex orientation

- on ne peut pas 'justify-self' car l'axe principal bouge comme un bloc

- pour 'pousser' un élément particulier qui se trouve sur l'axe principal, on peut utiliser un 'div class=push' avec une propriété de margin:auto:

```css
&__push {
  margin-left: auto;
}
```

- align-self: stretch est bien pour forcer une box à prendre toute la place

pour sass:

- il faut 'watch input output' pour que la compilation soit automatique

En général:

- créer une ombre, pas si facile. ajouter de la luminosité non plus. code de celle que j'ai créé

```css
.container {
  filter: drop-shadow(0 10px 0.75rem lighten(vars.$primary-bright, 30%));
}
```

- pour les images: il faut leur ajouter des bordures-radius manuellement, cover etc. ne prennent pas en compte les bordures.
- background-image fonctionne, mais requiert un wrapper. On peut s'en passer avec le code suivant (à noter aussi le border radius du point précédent):

```css
.image {
  height: 100%;
  width: vars.$widthMobile;
  object-fit: contain;
  border-radius: 25px 25px 0 0;
}
```

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
