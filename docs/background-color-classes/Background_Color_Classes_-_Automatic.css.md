# Background Color Classes - Automatic.css

**Source URL:** [https://automaticcss.com/docs/background-color-classes/](https://automaticcss.com/docs/background-color-classes/)  
**Last Updated:** 2025-05-22T21:46:19.212Z  
**Extracted:** 2025-05-31 16:57:06

---

# Background Color Classes - Automatic.css

Background classes allow you to change the background color on-the-fly, whether it’s a section, container, div, or any other boxed element.

While there are dozens of classes to choose from, they all follow the same conventions. If you remember the convention, you’ll be able to recall any color, shade, or transparency without having to look at the documentation.

## Main Color Convention

If you want to set the background color to one of the [main ACSS colors](https://automaticcss.com/docs/palette-setup/), use:

`.bg--[color]`

Example:

`<div class="bg--action"></div>`
Code language: HTML, XML (xml)

Any active color in your project will work.

## Shade Color Convention

If you want to set the background color to a shade of one of your colors, use:

`.bg--[color]-[shade]`

Example:

`<div class="bg--action-light"></div>`
Code language: HTML, XML (xml)

Shade values are ultra-light, light, medium, dark, ultra-dark, and hover.

## Transparency Color Convention

If you want to set the background color to a transparent version of one of your colors or shades, use:

`.bg--[color]-trans-[value]`  
`.bg--[color]-[shade]-trans-[value]`

Every main color offers transparent versions. Additionally, you can access transparencies of light, dark, and ultra-dark shades.

Example:

`<div class="bg--action-trans-20"></div>`
Code language: HTML, XML (xml)

`<div class="bg--action-ultra-dark-trans-20"></div>`
Code language: HTML, XML (xml)

Transparency values range from 10 to 90 in increments of 10.

## What about background patterns and gradients?

ACSS supports custom backgrounds, gradients, and overlays via our [Textures & Overlay](https://automaticcss.com/docs/textures-overlays/)s feature.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
