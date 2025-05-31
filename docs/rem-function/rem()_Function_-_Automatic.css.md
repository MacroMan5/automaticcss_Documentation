# rem() Function - Automatic.css

**Source URL:** [https://automaticcss.com/docs/rem-function/](https://automaticcss.com/docs/rem-function/)  
**Last Updated:** 2025-05-22T21:21:50.027Z  
**Extracted:** 2025-05-31 16:57:06

---

# rem() Function - Automatic.css

**Note:** Functions and mixins are designed for use in the Custom SCSS area of the Automatic.css dashboard. They will not work in the builder inputs or builder CSS.

ACSS often stores values without units to allow for certain types of calculations. Of course, to use the end result in a variable or a declaration, a unit is required. The rem() function attaches the rem unit to any number or variable.

For example, the $vp-max variable, which stores your website’s width value, is unitless. Let’s say you wanted to create a variable for a specific width, based on your website’s width. Here’s how you can use the rem() function with a simple calculation:

`$my-custom-width: rem($vp-max * .33);`
Code language: PHP (php)

This will create a variable equaling exactly 1/3 of your website’s width. If your website’s width is 1366, the end result will be 45.078rem if you’re set to 62.5% root font size and 27.173rem if your root font size is set to 100%.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
