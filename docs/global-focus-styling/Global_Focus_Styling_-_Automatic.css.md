# Global Focus Styling - Automatic.css

**Source URL:** [https://automaticcss.com/docs/global-focus-styling/](https://automaticcss.com/docs/global-focus-styling/)  
**Last Updated:** 2025-05-22T21:25:37.111Z  
**Extracted:** 2025-05-31 16:57:06

---

# Global Focus Styling - Automatic.css

Focus styling is when an element’s style is changed on [focus](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus) (when the user interacts with the element via keyboard, click, etc.). It’s a vital accessibility feature so users know which particular clickable element they’re interacting with.

Websites don’t have focus styling by default – the developer must add it. Or, in this case, a tool like Automatic.css adds it for you (yet another thing you don’t have to remember!).

## Customizing Focus Styling

![ACSS Focus Styling Panel](https://automaticcss.com/wp-content/uploads/CleanShot-2023-08-15-at-09.34.12@2x-1024x487.jpg)

You can customize your site’s focus styling in the ACSS Additional Styling panel under Accessibility.

### Focus Style

Choose between Outline or Shadow. Outline uses the CSS [outline](https://developer.mozilla.org/en-US/docs/Web/CSS/outline) property. Shadow uses the [Box Shadow](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow) property.

The advantage of `outline` is the ability to offset the focus ring from the element in focus. The advantage of the `box-shadow` method is that the box shadow will follow curves of elements being focused (where `outline` will put a square around rounded elements in many browsers).

### Focus Color

You can choose any color for your focus color. The default is your website’s action color.

Remember that you can change the focus color of individual elements using [focus classes](https://automaticcss.com/docs/focus-classes/).

### Focus Width

This setting allows you to control the thickness of the focus indicator. Rem units are a good choice here.

### Focus Offset

This setting is only available when the outline focus style is chosen. It allows you to control the amount of offset – the gap between the focus indicator and the element being focused.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
