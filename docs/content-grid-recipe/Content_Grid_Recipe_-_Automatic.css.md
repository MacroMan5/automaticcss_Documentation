# Content Grid Recipe - Automatic.css

**Source URL:** [https://automaticcss.com/docs/content-grid-recipe/](https://automaticcss.com/docs/content-grid-recipe/)  
**Last Updated:** 2025-05-22T21:46:19.520Z  
**Extracted:** 2025-05-31 16:57:06

---

# Content Grid Recipe - Automatic.css

You can deploy a [content grid layout](https://automaticcss.com/docs/content-grid/) to any box with the `@content-grid;` recipe.

`@content-grid;`
Code language: CSS (css)

This recipe automatically outputs the `%root%` selector so you can deploy it directly in the CSS box without any preparation.

Once deployed, you can assign things to different zones using the `grid-column` property:

`.my-awesome-grid > :is(figure, picture, img) {   grid-column: feature; }`
Code language: CSS (css)

The above example assigns all figure elements, picture elements, and images to the “feature” zone.

You can also still use all the content grid `.feature--` utility classes, assuming you have them turned on.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
