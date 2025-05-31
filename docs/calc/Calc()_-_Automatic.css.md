# Calc() - Automatic.css

**Source URL:** [https://automaticcss.com/docs/calc/](https://automaticcss.com/docs/calc/)  
**Last Updated:** 2025-05-22T21:21:48.613Z  
**Extracted:** 2025-05-31 16:57:06

---

# Calc() - Automatic.css

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

The `calc()` function is a standard CSS function that’s not proprietary to Automatic.css. However, this documentation outlines our recommendation for using `calc()` in conjunction with ACSS variables in your workflow.

## Text & Spacing “Tweener” Sizes

It’s common to need a size in-between what’s available by default in ACSS for text and spacing utilities. You have two options in these cases. You can [create a brand new custom property with `fluid()`](https://automaticcss.com/docs/fluid-function/) or you can quickly use `calc()` and move on. In the majority of cases, `calc()` is probably just fine.

For example, let’s say I’m building a card and I want half of my normal [content gap](https://automaticcss.com/docs/contextual-spacing/). Rather than making a custom variable, I can simply do this:

`gap: calc(var(--content-gap) / 2);`
Code language: JavaScript (javascript)

Of course, you could create a brand new custom property using the calc function also:

`:root {   --card-gap: calc(var(--content-gap) / 2); }`
Code language: CSS (css)

There’s really no right or wrong here, but using a raw `calc()` function is definitely the quickest and easiest approach. The other approaches would be good if you find yourself repeating the same `calc()` over and over again.

## Colors

You can calc() colors to manipulate existing colors or create news. For example, let’s say I wanted to reduce the saturation of my primary color by 20% and assign that to a new custom property. I can do this:

`:root {   --primary-trans-5: hsl(var(--primary-h) calc(var(--primary-s) / .2) var(--primary-l)) }`
Code language: CSS (css)

Here’s a breakdown:

*   `hsl()` – Declare a new HSL value.
*   `var(--primary-h)` – Reference the primary color’s hue value.
*   `calc(var(--primary-s) / .2)` – Reference the primary color’s saturation value and reduce it by 20% using `calc()`.
*   `var(--primary-l)` – Reference the primary color’s lightness value.

This is covered in more detail in [Palette Setup](https://automaticcss.com/docs/palette-setup/).

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
