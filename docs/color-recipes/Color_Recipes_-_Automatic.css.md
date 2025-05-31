# Color Recipes - Automatic.css

**Source URL:** [https://automaticcss.com/docs/color-recipes/](https://automaticcss.com/docs/color-recipes/)  
**Last Updated:** 2025-05-22T21:41:30.622Z  
**Extracted:** 2025-05-31 16:57:06

---

# Color Recipes - Automatic.css

Color recipes are shortcuts for exposing the full string behind a given color. For example, @primary-clr will expand to:

`hsl(var(--primary-h) var(--primary-s) var(--primary-l) / 1)`
Code language: JavaScript (javascript)

This allows you to manipulate any part of the HSL string on the fly with custom values or calcs. Also notice that the expansion includes the alpha channel, making it super easy to create custom transparencies.

All colors and shades are available using the syntax:

*   Color: `@{color-name}-clr`
*   Shade: `@{color-name}-{shade}-clr`

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
