# “Is Background” (.is-bg) - Automatic.css

**Source URL:** [https://automaticcss.com/docs/is-background-is-bg/](https://automaticcss.com/docs/is-background-is-bg/)  
**Last Updated:** 2025-05-22T21:35:26.414Z  
**Extracted:** 2025-05-31 16:57:06

---

# “Is Background” (.is-bg) - Automatic.css

3.2.10

It’s a very common requirement in web design to take an element and place it in the background. Or, more commonly, _as_ the background.

Doing this requires specific CSS on the element in question as well as CSS changes to the direct parent of the element.

In Automatic.css, it’s achieved with one simple utility class: `.is-bg`.

## Making a real image a background image

Advanced developers often want to use real images as background images instead of using the CSS `background-image` property. This is because real images have a number of advantages: they’re indexable, they’re compatible with lazy load, they can have alt tags, they’re compatible with src-set, you can make use of the `<picture>` tag, and so on.

To make a real image a background image with ACSS, add an image element to the page (often in a section), and then add `.is-bg` to the image.

That’s all there is to it.

Now you can add additional classes to the image, like [overlay classes](https://automaticcss.com/doc-cat/overlays/), [object-position classes](https://automaticcss.com/docs/object-fit-classes/), [flip classes](https://automaticcss.com/docs/flip-classes/), [opacity classes](https://automaticcss.com/docs/opacity-classes/), etc.

## Make any box a background

`.is-bg` is compatible with almost any element. This means you can take a blank box and make it a background. Then you can style the box however you’d like.

If you add a blank box with `.is-bg` immediately after your image that’s also using `.is-bg`, the box will act as an overlay on that image. You can actually stack layers indefinitely like this.

## How `.is-bg` works

The utility works by positioning the element absolutely, forcing its dimensions to match the exact dimensions of its parent, and setting the z-index to `-2` for infinite layering without affecting content or other features like overlay which occupy the `-1` layer.

It also identifies the direct parent, sets the `position` to `relative` and creates a new stacking context using `isolation`.

All values for `.is-bg` are tokenized, with the real values being added as fallbacks. This means you can interact-with and easily override any of the `.is-bg` tokens:

*   `--bg-position` – defaults to absolute
*   `--bg-inset` – defaults to 0
*   `--bg-width` – defaults to 100%
*   `--bg-height` – defaults to 100%
*   `--bg-radius` – defaults to 0
*   `--bg-z-index` – defaults to -2
*   `--bg-object-fit` – defaults to cover (only applies to images)
*   `--bg-object-position` – defaults to center (only applies to images)

Yes, this means you can also get creative with how your background elements behave/appear/animate.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
