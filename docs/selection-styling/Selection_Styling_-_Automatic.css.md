# Selection Styling - Automatic.css

**Source URL:** [https://automaticcss.com/docs/selection-styling/](https://automaticcss.com/docs/selection-styling/)  
**Last Updated:** 2025-05-22T21:27:29.049Z  
**Extracted:** 2025-05-31 16:57:06

---

# Selection Styling - Automatic.css

ACSS users can control the background and foreground color of selected text (highlighted when the user clicks and drags to select text on the site) via the Selection Styling panel under Additional Styling.

![Selection Styling Options](https://automaticcss.com/wp-content/uploads/CleanShot-2024-10-20-at-08.58.17@2x-1024x882.jpg)

Selection Styling Options

The first two fields define the default selection styling for the website. The second two fields define an alternate selection style, for when the main selection style might not be appropriate (primary colored selection text on a primary colored background, for example).

As always, color tokens are recommended here. Users should avoid using raw color values or keywords, especially if you want to retain compatibility with [color scheme](https://automaticcss.com/docs/color-scheme-dark-mode/).

To use the alternate selection style, place the `.selection--alt` class on any box. This will affect all children of the box as well.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
