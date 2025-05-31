# ctr() Function - Automatic.css

**Source URL:** [https://automaticcss.com/docs/ctr/](https://automaticcss.com/docs/ctr/)  
**Last Updated:** 2025-05-22T21:21:49.117Z  
**Extracted:** 2025-05-31 16:57:06

---

# ctr() Function - Automatic.css

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

Sometimes you need to convert a pixel value to rem. If you’re needing to do this in a builder input or custom CSS input, you can simply use our [convert to rem expansion feature](https://automaticcss.com/docs/prem/). If, however, you’re writing custom SCSS and need to convert a pixel value to rem, you can use the `ctr()` function (ctr = convert to rem).

`.my-static-spacing-value {   padding: ctr(24); }`
Code language: CSS (css)

The above example will take 24px and convert it to rem based on your website’s root font size.

Please remember that you can’t use functions within `:root`, so if you need to use this function to define a new custom property, you first need to create a SCSS variable and then interpolate it in `:root`:

`$my-custom-value: ctr(24); :root {   --my-custom-value: #{$my-custom-value}; }`
Code language: PHP (php)

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
