# Button Variables - Automatic.css

**Source URL:** [https://automaticcss.com/docs/button-variables/](https://automaticcss.com/docs/button-variables/)  
**Last Updated:** 2025-05-22T21:26:17.318Z  
**Extracted:** 2025-05-31 16:57:06

---

# Button Variables - Automatic.css

There may be times when you want to design your own custom button, but you still want to use specific values from ACSS’s global button settings. If this is the case, you can use button variables.

The following button variables can be changed at any time with custom styling:

*   `--btn-background`
*   `--btn-background-hover`
*   `--btn-text-color`
*   `--btn-text-color-hover`
*   `--btn-text-transform`
*   `--btn-text-decoration`
*   `--btn-text-decoration-hover`
*   `--btn-letter-spacing`
*   `--btn-line-height`
*   `--btn-font-size`
*   `--btn-font-weight`
*   `--btn-font-style`
*   `--btn-padding-block` (top and bottom padding)
*   `--btn-padding-inline` (left and right padding)
*   `--btn-min-width`
*   `--btn-transition-duration`
*   `--btn-border-color`
*   `--btn-border-color-hover`
*   `--btn-border-style`
*   `--btn-radius`
*   `--btn-border-width`
*   `--btn-outline-background-color`
*   `--btn-outline-border-hover`
*   `--btn-outline-border-width`
*   `--btn-outline-text-color`
*   `--btn-outline-text-color-hover`
*   `--focus-color`

## Deprecated Button Variables

The following variables are still loaded in the framework but are considered officially deprecated. You should stop using them on future projects and start using the new variables above.

*   `--btn-border-size`
*   `--outline-btn-border-size`
*   `--btn-pad-x`
*   `--btn-pad-y`
*   `--btn-text-style`
*   `--btn-text-size`
*   `--btn-weight`
*   `--btn-width`

## Example custom button

Let’s say we want to create a button that shares all the same general styling as our default buttons but has a gradient background instead of a solid background:

`.gradient-button {   background: linear-gradient(var(--action-medium), var(--action));  padding: var(--btn-padding-block) var(--btn-padding-inline);  font-size: var(--btn-font-size);  line-height: var(--btn-line-height);  letter-spacing: var(--btn-letter-spacing);  border-width: var(--btn-border-width);  border-style: var(--btn-border-style);  border-radius: var(--btn-border-radius);  border-color: transparent;  font-weight: var(--btn-font-weight);  text-decoration: var(--btn-text-decoration);  font-style: var(--btn-font-style);  text-transform: var(--btn-text-transform);  min-inline-size: var(--btn-min-width);  transition: background var(--btn-transition-duration) ease-in-out; }`
Code language: CSS (css)

Now you have a custom gradient button that will still inherit any changes you make to your global button styles in the ACSS dashboard.

Additionally, if you’re using SCSS, you can use our [button mixin](https://automaticcss.com/docs/button-mixins/) to apply all the default styles in one line automatically.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
