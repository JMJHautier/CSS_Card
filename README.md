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

#### Pour flexbox:

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

#### pour sass:

- il faut 'watch input output' pour que la compilation soit automatique

#### En général:

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

# Frontend Mentor - Order summary card

![Design preview for the Order summary card coding challenge](./design/desktop-preview.jpg)

## Welcome! 👋

Thanks for checking out this front-end coding challenge.

[Frontend Mentor](https://www.frontendmentor.io) challenges help you improve your coding skills by building realistic projects.

**To do this challenge, you need a basic understanding of HTML and CSS.**

## The challenge

Your challenge is to build out this order summary card component and get it looking as close to the design as possible.

You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.

Your users should be able to:

- See hover states for interactive elements

Want some support on the challenge? [Join our Slack community](https://www.frontendmentor.io/slack) and ask questions in the **#help** channel.

## Where to find everything

Your task is to build out the project to the designs inside the `/design` folder. You will find both a mobile and a desktop version of the design.

The designs are in JPG static format. Using JPGs will mean that you'll need to use your best judgment for styles such as `font-size`, `padding` and `margin`.

If you would like the design files (we provide Sketch & Figma versions) to inspect the design in more detail, you can [subscribe as a PRO member](https://www.frontendmentor.io/pro).

You will find all the required assets in the `/images` folder. The assets are already optimized.

There is also a `style-guide.md` file containing the information you'll need, such as color palette and fonts.

## Building your project

Feel free to use any workflow that you feel comfortable with. Below is a suggested process, but do not feel like you need to follow these steps:

1. Initialize your project as a public repository on [GitHub](https://github.com/). Creating a repo will make it easier to share your code with the community if you need help. If you're not sure how to do this, [have a read-through of this Try Git resource](https://try.github.io/).
2. Configure your repository to publish your code to a web address. This will also be useful if you need some help during a challenge as you can share the URL for your project with your repo URL. There are a number of ways to do this, and we provide some recommendations below.
3. Look through the designs to start planning out how you'll tackle the project. This step is crucial to help you think ahead for CSS classes to create reusable styles.
4. Before adding any styles, structure your content with HTML. Writing your HTML first can help focus your attention on creating well-structured content.
5. Write out the base styles for your project, including general content styles, such as `font-family` and `font-size`.
6. Start adding styles to the top of the page and work down. Only move on to the next section once you're happy you've completed the area you're working on.
