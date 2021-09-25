# Styles folder

_You do not have to use this structure, or place your styles here! But it's a good and common practice, and these folders are ones you'll reasonably end up using throughout the course of this project._

## Recommended reading:

- [General best practices for writing styles](https://medium.com/before-semicolon/50-css-best-practices-guidelines-to-write-better-css-c60807e9eee2)
- [7-1 folder structure for SASS projects](https://www.learnhowtoprogram.com/user-interfaces/building-layouts-preprocessors/7-1-sass-architecture) - whether or not to use a preprocessor is up to you, but it's good reading for if you do.
- [BEM (Block/Element/Modifier) overview](http://getbem.com/introduction/) - normally I wouldn't bother with this for a project this size, but it could be fun to try! Good practice, too.

## Directory overview

- `/components` is for styles that can be called in to a specific discrete component. This can either be a framework component (like a React or Vue component) or it can be eg `.notification` that can style any plain old div into a snackbar notification.
- `/config` is for any files that configure the styles globally - for example, a CSS normalizer file, or a SCSS global variables file.
- `/fonts` to store fonts, if not using an online font service like Google Fonts. Could also store an icon font here :)
- `/layout` stores styles for pieces like your site header, your navigation, and anything else that's pretty universal - for example, the base styles for your site. (You could, though, store the styles for a subheader that's used in the Blog section of the site here, for example)
- `/pages` for any page-specific styles, eg your home page might have a hero bar, and a "meet our team" section, which won't be used anywhere else.
- `/utilities` if for helpful styles that can be applied at will to tweak an existing style without having to write a whole new one - for example, `.no-border` or `.color-active` or `.padding-md` or `.display-inline` or `.display-flex` or `.display-fixed`. Depending on how many of these you have, you can decide to have them all in one file, or break them up so you don't have to load the whole thing on each page if you just need one item. Be careful - if you find yourself using these a lot, you probably need an actual style for it written in an appropriate place!

Note that there are no solid rules. It all depends on your use case, and where the project is going. The `.validation-modal` styles, for example, would be in `/components` if you foresaw other similar validation modals being used sitewide - otherwise, it would probably be in `/pages/cart.css`...

## Mobile

If you're doing the extra challenge to create a mobile version, remember to do the mobile version first - selectively _adding_ styles is a lot easier than taking them away!
