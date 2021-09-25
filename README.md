# Shopping Cart CSS Challenge - Sept 2021

## Overview

I have created some HTML scaffolding, including example class names and the text shown in the mockup. I have used semantic html where possible, and followed the general rule of "use classes instead of element selectors" to prevent over-specificity. You don't have to use any of this, but it should save you some time!

I have included a copy of the spec, and a screenshot of the page where every element has a border and padding, to help visualize how the elements come together.

## Extra credit

- Create a mobile version. Remember that there isn't a mobile spec to work off of! You'll have to design it! I have set up the scaffolding so you shouldn't have any trouble making the layout work on mobile.
- Make it work in IE 11 :P
- Make it accessible - include aria labels, a high-contrast mode, tab navigation, etc.
- Include some relevant `<meta>` tags!

## Hints

- You may want to overwrite some styles on buttons, inputs, and headers
- Remember that grid items automatically line up with each other
- If doing mobile - remember that you can specify an item's grid position in the CSS, while flex items are more FLEXible (sorry)
- `::after` and `::before` are super handy! So is the `text-overflow` property ;)
- Sometimes designers don't know how things work....
- General gotcha about positioning using `absolute`, `relative`, and `fixed` - an absolute item inside a relative item will be absolute WITHIN THE BOUNDS of its parent element. You can use this to your advantage.
- General gotcha about `z-index`: z-index is set WITHIN THE CONTEXT of its siblings!! In the below, 'Hello!' would show up above '(hello)' but not above 'HELLO!!!' (because the second div has a higher z-index). You can also use this to your advantage!

        <div style="z-index: 1">
            <p style="z-index: 100">Hello!</p>
            <p style="z-index: 1">(hello)</p>
        </div>
        <div style="z-index: 2">
            <p style="z-index: 50">HELLO!!!</p>
        </div>

- Note the gradient on the left edge of the card details pane, and the subtle pink-orange blush over the grey of the background of that pane.
