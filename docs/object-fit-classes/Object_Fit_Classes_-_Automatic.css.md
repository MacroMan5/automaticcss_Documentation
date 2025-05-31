# Object Fit Classes - Automatic.css

**Source URL:** [https://automaticcss.com/docs/object-fit-classes/](https://automaticcss.com/docs/object-fit-classes/)  
**Last Updated:** 2025-05-22T21:37:26.712Z  
**Extracted:** 2025-05-31 16:57:06

---

# Object Fit Classes - Automatic.css

There are situations where you need to set a width, [height](https://automaticcss.com/docs/height-classes/), or [aspect ratio](https://automaticcss.com/docs/aspect-ratio-classes/) on an image that doesn’t respect the image’s original aspect ratio. When this occurs, the image “stretches” and looks warped.

**Object Fit** classes force the image to look appropriate in the new aspect ratio by cropping into the image (`.object-fit--cover`). Or, they force it back to its original aspect ratio within the new container bounds (`.object-fit--contain`).

Note: “Contain” is similar to the technique of letterboxing in video production. It’s used far less often than “cover.”

As is true with background images, you can also choose which area of the image to preserve (`.object-fit--[area]`) with “area” being one of the following named coordinates:

*   top-left
*   top-center
*   top-right
*   center-left
*   center-right
*   bottom-left
*   bottom-center
*   bottom-right

Note: There’s no center-center option because that’s the default position of object-fit.

Here’s an example of how and when to use object-fit classes:

`<img class="aspect--16-9 object-fit--cover object-fit--center-right" src="sample-image.jpg" />`
Code language: JavaScript (javascript)

In the above example `.aspect--16-9` changes the aspect ratio of the image to 16×9. The image had an original aspect ratio of 6×4, thus we need to use object-fit to prevent improper stretching. The class `.object-fit--cover` establishes that we want to use the cover method (cropping) and .`object-fit--center-right` instructs the browser to preserve the right-most side of the image when cropping.

Notice how all three classes are used simultaneously to achieve the desired outcome.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
