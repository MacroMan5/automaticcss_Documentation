# Card Container Recipe - Automatic.css

**Source URL:** [https://automaticcss.com/docs/card-container-recipe/](https://automaticcss.com/docs/card-container-recipe/)  
**Last Updated:** 2025-05-22T21:43:09.205Z  
**Extracted:** 2025-05-31 16:57:06

---

# Card Container Recipe - Automatic.css

The Card Container recipe is used for adding container queries to card styling by the ACSS [Card Framework](https://automaticcss.com/docs/card-framework/).

You can deploy it by typing `@card-container;` in the custom CSS area.

To use the recipe, you must do two things:

1.  Define the size parameters in the parenthesis. You can use any standard media query size syntax as well as the new [range syntax](https://css-tricks.com/the-new-css-media-query-range-syntax/).
2.  Add your custom CSS.

Pro Tip: Instead of redeclaring properties like padding, font-size, etc. just declare new values for the custom properties that are used throughout the card framework.

## Nesting Styles

Native CSS now supports nesting, which you can leverage to keep all your container query CSS inside a single query (unless you’re designing for multiple size contexts).

## Example

`%root% {    @container card ( inline-size >= 767px ) {      display: grid;      grid-template-columns: var(--grid-2-3);      --card-media-aspect-ratio: 4/3;      --card-heading-size: var(--h2);   } }`
Code language: JavaScript (javascript)

The above code changes the card to a 2-3 grid, changes the aspect ratio of the card media, and changes the card heading size to the H2 size when the card is in a container that’s greater-than or equal-to 767px.

If you prefer to use a Mixin for this, you can use the [Card Container Mixin](https://automaticcss.com/docs/card-container-mixin/).

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
