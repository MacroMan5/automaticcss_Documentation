# Centering Mixin - Automatic.css

**Source URL:** [https://automaticcss.com/docs/center-mixin/](https://automaticcss.com/docs/center-mixin/)  
**Last Updated:** 2025-05-22T21:23:24.408Z  
**Extracted:** 2025-05-31 16:57:06

---

# Centering Mixin - Automatic.css

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

Automatic.css’ [centering classes](https://automaticcss.com/docs/centering-classes/) are powered by the `center()` mixin, which is also available for users to use on their own. Here’s what it looks like

`@include center($alignment, $output);`
Code language: PHP (php)

The `center()` mixin accepts two arguments: `$alignment` and `$output`.

The $alignment argument accepts all the same alignments that are available with the [centering classes](https://automaticcss.com/docs/centering-classes/):

*   `all` – center across both axes
*   `left` – center vertically, align left
*   `right` – center vertically, align right
*   `top` – center horizontally at the top
*   `bottom` – center horizontally at the bottom

The $output arguments accepts:

*   `full` – The full output
*   `core` – The flex properties output only
*   `tokens` – The tokens/values output only

It’s important to note that the `$alignment` argument defaults to “all” and the `$output` argument is not required.

If you want to center everything, it’s as easy as this (since “all” is the default):

`.my-centered-box {   @include center; }`
Code language: PHP (php)

Here’s an example of centering vertically, but aligning left:

`.my-centered-box {   @include center(left); }`
Code language: PHP (php)

And here’s an example of how to set initial centering and then manipulate it at a breakpoint using [breakpoint mixins](https://automaticcss.com/docs/breakpoint-mixins/):

`.my-centered-box {   @include center;   @include breakpoint(l) {    @include center(left, tokens);  } }`
Code language: PHP (php)

In the above example, the “tokens” output is all you need at each breakpoint when you’ve already established the full output for the current selector (by using the mixin once already). This is because the tokens output sets new values for the properties that already exist without repeating everything again. It’ll work even if you don’t use the “tokens” output, but the tokens output is more efficient.

## Why is my selector output twice?

When using the `center()` mixin, you’ll notice a double selector output. This is normal – the mixin is designed to double the selector to increase specificity and improve compatibility with various page builders.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
