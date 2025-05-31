# Button Mixins - Automatic.css

**Source URL:** [https://automaticcss.com/docs/button-mixins/](https://automaticcss.com/docs/button-mixins/)  
**Last Updated:** 2025-05-22T21:26:46.216Z  
**Extracted:** 2025-05-31 16:57:06

---

# Button Mixins - Automatic.css

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

It’s common to use 3rd party plugins on WordPress websites or run into scenarios where you need to apply button styling to specific elements that you can’t necessary apply a button class to.

Some of these plugins, like e-commerce plugins, form plugins, etc. contain buttons that need to match the style of all your other buttons. This is a perfect use case for a button mixin.

Note: Button mixins are part of ACSS’ SCSS structure, so they can’t be used in regular CSS fields. You’ll need to use the mixin in the Custom SCSS area of the ACSS dashboard.

## `btn()`

The main button mixin in ACSS is the `btn()` mixin. This mixin allows you to attach any ACSS button style to any link/button element you’d like. You can use it like this:

`.target-button-element {   @include btn(primary); }`
Code language: PHP (php)

The above code will make `.target-button-element` exactly match your website’s primary button style.

### Available Styles

You can replace “primary” in the above example with any valid ACSS button style:

*   primary
*   primary-light
*   primary-dark
*   primary.btn–outline
*   primary-light.btn–outline
*   primary-dark.btn–outline
*   secondary
*   secondary-light
*   secondary-dark
*   secondary.btn–outline
*   secondary-light.btn–outline
*   secondary-dark.btn–outline
*   tertiary
*   tertiary-light
*   tertiary-dark
*   tertiary.btn–outline
*   tertiary-light.btn–outline
*   tertiary-dark.btn–outline
*   accent
*   accent-light
*   accent-dark
*   accent.btn–outline
*   accent-light.btn–outline
*   accent-dark.btn–outline
*   base
*   base-light
*   base-dark
*   base.btn–outline
*   base-light.btn–outline
*   base-dark.btn–outline
*   neutral
*   neutral-light
*   neutral-dark
*   neutral.btn–outline
*   neutral-light.btn–outline
*   neutral-dark.btn–outline

Note: To use the `.btn--outline` versions, you’ll need to wrap the entire style name in quotes, like this:

`.target-button-element {   @include btn("primary.btn--outline"); }`
Code language: PHP (php)

## Dealing With Specificity Issues

In the above example, `.target-button-element` could be an element that already has styles applied to it. If these styles contain greater specificity than your CSS instructions, or are placed in a stylesheet that comes after ACSS’ custom CSS, the mixin won’t work unless you increase specificity.

One way you can increase specificity without actually altering HTML is to double-reference the selector, like this:

`.target-button-element.target-button-element {   @include btn("primary.btn--outline"); }`
Code language: PHP (php)

Another way you can increase specificity is to use a page builder’s html/body/main ID (if one exists) to start your CSS declaration. For example, Bricks uses an ID on their main tag, so you can use it to increase specificity without altering HTML, like this:

`#brx-content .target-button-element {   @include btn("primary.btn--outline"); }`
Code language: PHP (php)

If the mixin isn’t working for some reason, or is partially working, you’ll need to calculate the specificity of the default styles you’re trying to override, and then produce higher specificity with your mixin targeting.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
