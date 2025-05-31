# Heading & Text Style Mixins - Automatic.css

**Source URL:** [https://automaticcss.com/docs/heading-text-style-mixins/](https://automaticcss.com/docs/heading-text-style-mixins/)  
**Last Updated:** 2025-05-22T21:40:42.425Z  
**Extracted:** 2025-05-31 16:57:06

---

# Heading & Text Style Mixins

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

Note: Mixins only work within the custom SCSS area of the ACSS dashboard.

## Heading Styles

You can apply any heading level’s global styles to a custom selector using `@heading-style();`

`.custom-heading {   @include heading-style(h2); }`
Code language: PHP (php)

This will attach all global heading styles as well as any styles specific to the heading level you reference, but will not output any properties that have a null value.

### Text Styles

You can apply any text level’s global styles to a custom selector using `@text-style();`

`.custom-text {   @include text-style(l); }`
Code language: PHP (php)

This will attach all global text styles as well as any styles specific to the text level you reference, but will not output any properties that have a null value.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
