# Gradient Fades - Automatic.css

**Source URL:** [https://automaticcss.com/docs/gradient-fades/](https://automaticcss.com/docs/gradient-fades/)  
**Last Updated:** 2025-05-22T21:23:23.721Z  
**Extracted:** 2025-05-31 16:57:06

---

# Gradient Fades - Automatic.css

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

It’s common to need to fade out content into the background. And in an ideal world, you don’t want to have to match the fade color effect with the background color. Rather, you want the fade out to work regardless of color choices, background textures, etc.

This is precisely what ACSS’ Gradient Fades feature handles for you. You can see an example of this in the [Frames](https://getframes.io/) layout, [Hero Barcelona](https://getframes.io/layouts/hero-barcelona/).

Note: If you don’t have a Frames license, you should definitely [get one here](https://getframes.io/pricing/).

![](https://automaticcss.com/wp-content/uploads/CleanShot-2025-02-28-at-16.29.02@2x-1024x487.webp)

As you can see in the above example, the images appear to fade into the background of the section. This is accomplished with ACSS’ fade utilities.

## Getting Started

The fade effect can be applied with **fade utility classes**, the **fade() mixin**, or **fade recipes**.

If you want to use the utility classes, make sure they’re activated in **Options > Utility Classes > Fade Classes**.

The recipe and mixin() are available at all times, even when the utility classes are deactivated.

## Fade Utility Classes

Apply classes using the syntax `.fade--{axis}`. The accepted axis extensions are: `block`, `inline`, `top`, `right`, `bottom`, `left`.

“Block” fades out both sides of the block axis. “Inline” fades out both sides of the inline access. The others do exactly what you’d expect them to do.

Once applied, you can adjust the fade amount using a locally scoped variable `--fade-amount`, either on a custom class or at the ID level.

`.foo {   --fade-amount: 35%; }`
Code language: CSS (css)

## Fade Mixin

The fade mixin works in the custom SCSS area of the ACSS dashboard. Choose and element and `@include fade($axis, $amount)`.

`.foo {   @include fade(block, 35%); }`
Code language: PHP (php)

The `$amount` argument is not required. It will default to 25%.

## Fade Recipes

Each axis option has an associated recipe. The following will expand the fade out code:

*   `@fade-block;`
*   `@fade-inline;`
*   `@fade-top;`
*   `@fade-right;`
*   `@fade-bottom;`
*   `@fade-left;`

Remember that you can’t paste these recipe strings. They’ll only expand when the semicolon on the end is actually typed.

That’s it, have fun!

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
