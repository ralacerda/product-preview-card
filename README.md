# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot_desktop.png)
![](./screenshot_mobile.png)

### Links

- [Solution URL](https://github.com/ralacerda/product-preview-card)
- [Live Site URL](https://ralacerda.github.io/product-preview-card/)

## Built with

- Semantic HTML5 markup
- CSS variables
- Flex and Grid
- CUBE CSS

I used a grid layout to place the photo and the product description side by side on the desktop version, changing the flow to `column` in the mobile version.

Flex was used to center elements and set gaps, which was really helpful.

Using CUBE `flow` component class was really helpful, clear way to set a margin top for all but the first child:

```
.flow > * + * {
  margin-top: 21px;
}
```

In this challenge, I didn't override the margin-top for the child elements, so I didn't had to set a variable with defaults.

I took me around 3 hours to finish it.

### What I learned

Took a while to wrap my head around CUBE methodology, which I'm sure I did not follow 100%. I did enjoy using utility classes, which is similar to who tailwind works, but for this simple challenge it was hard to decide what would be a utility class and what I should style as a block.

I also noticed you have to place your media-query AFTER the values you are trying to override.

Placing the same prices on the same vertical level was annoying, but I think using flex was a good solution in the end.

### Continued development

The CSS is far from perfect, and while I was not following CUBE 100%, I think it helped me create cleaner CSS.

The result is not pixel perfect, but I'm happy with it.

In real production code, I would use more variables and utility classes, since they are really helpful for changing code later and re-using classes.

## Author

- Github - [Renato Lacerda](https://github.com/ralacerda)
- Frontend Mentor - [@ralacerda](https://www.frontendmentor.io/profile/ralacerda)
