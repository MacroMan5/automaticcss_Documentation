# Content Grid Mixin - Automatic.css

**Source URL:** [https://automaticcss.com/docs/content-grid-mixin/](https://automaticcss.com/docs/content-grid-mixin/)  
**Last Updated:** 2025-05-22T21:23:25.812Z  
**Extracted:** 2025-05-31 16:57:06

---

# Content Grid Mixin - Automatic.css

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

You can deploy a [content grid layout](https://automaticcss.com/docs/content-grid/) to any box with the `content-grid()` mixin.

`.my-awesome-grid {   @include content-grid; }`
Code language: PHP (php)

This is an argument-less mixin that’s essentially plug and play. Once you’ve applied it to a box, you can assign children to content grid zones using the `grid-column` property.

`.my-awesome-grid > :is(figure, picture, img) {   grid-column: feature; }`
Code language: CSS (css)

The above example assigns all figure elements, picture elements, and images to the “feature” zone.

You can also still use all the content grid `.feature--` utility classes, assuming you have them turned on.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
