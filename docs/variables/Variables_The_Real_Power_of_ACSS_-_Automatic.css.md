# Variables: The Real Power of ACSS - Automatic.css

**Source URL:** [https://automaticcss.com/docs/variables/](https://automaticcss.com/docs/variables/)  
**Last Updated:** 2025-05-22T21:20:03.316Z  
**Extracted:** 2025-05-31 16:57:06

---

# Variables: The Real Power of ACSS

Variables, or “custom properties” in CSS, are the modern standard for assigning values. Variables make web development more efficient, consistent, and maintainable.

ACSS was one of the first utility frameworks to encourage using variables while giving users an entire library of variables that perfectly map to utility classes. And really, ACSS variables are the most potent aspect of Automatic.css.

## How variables work

A variable in CSS is just a token, or placeholder, for a value.

Here’s a typical scenario where you need to set the background color of a card:

`.my-card {    background-color: #08001F; }`
Code language: CSS (css)

That color isn’t random. It is a dark color commonly used across many parts of our example website, which means it’s referenced over and over again.

Using the hex code is undesirable because:

1.  Hex codes are hard to remember. You’ll probably need to look it up whenever you use it.
2.  If the color changes in the future, you’ll have to change the hex code everywhere it was used manually.
3.  Hex codes can’t be changed dynamically based on certain conditions.
4.  Hex codes can’t be manipulated. For example, you can’t set alpha transparency, adjust its hue, adjust its saturation, or adjust its lightness.

It’s better to use a variable here because a variable solves all these common challenges.

`.my-card {    background-color: var(--base-dark); }`
Code language: CSS (css)

`--base-dark` is the variable, but it must be wrapped in a `var()` function to use it.

At first, this takes a little getting used to, but the learning curve is relatively flat. After a few times, it’ll become second nature.

## How do variables get their values?

Values are assigned to variables in one of two places:

*   At the site’s `:root` level (global variables)
*   At the element/class level (local variables)

In Automatic.css, all variables are defined for you at the `:root` level making them available site-wide by default. They map to all of your chosen values in the ACSS dashboard. There are variables for colors, font sizes, border radius, spacing, and more.

[Open the cheat sheet](https://automaticcss.com/cheat-sheet/) and filter the utility type to “variable” to see all available variables.

## How & when to use a variable in ACSS

Variables should be used when you create a custom class for an element. This is common in situations where you want to maintain global control over an element’s styling. Thus you don’t want to use utility classes.

Here’s a great video that will help you understand when to use utility classes vs custom classes:

Utility Classes vs Custom Classes in ACSS (Best Practices) - YouTube

[](https://www.youtube.com/watch?v=bNzWVAPlMgU&embeds_referring_euri=https%3A%2F%2Fautomaticcss.com%2F)

When using a custom class, it means you will assign values for different CSS properties manually. For example, we need to define padding for our example card above.

`.my-card {    background-color: var(--base-dark);   padding: var(--space-l); }`
Code language: CSS (css)

We could very easily choose a random value for our spacing (e.g. 3em), but then we’d lose many benefits of the ACSS variable, namely consistency and automatic responsiveness.

## Overriding variables with local values

A key benefit of using global variables is that you can change the variable’s value at any time and it’ll apply everywhere that variable has been used. There’s another benefit, though – the ability to override a variable’s value in specific places.

Let’s say that “my-card” is being used in a specific place where we want to change its text color and background color.

Here’s the code we have our card so far:

`.my-card {    background-color: var(--base-dark);   color: var(--white);   padding: var(--space-l); }`
Code language: CSS (css)

All we need to do is give our tokens new values. We just have to do this within a specific context, like when there’s a specific data attribute present:

`[data-theme-style="secondary"] .my-card {    --base-dark: var(--secondary);   --white: var(--secondary-ultra-dark); }`
Code language: CSS (css)

This would change the value of `--base-dark` to whatever the value of our `--secondary` color is. And it would change the text color from `--white` to whatever the value of `--secondary-ultra-dark` is.

You could also do this with a modifier class:

`.my-card--secondary {    --base-dark: var(--secondary);   --white: var(--secondary-ultra-dark); }`
Code language: CSS (css)

You could also do it to a single card by applying this technique at the ID level:

`#my-card-3125 {    --base-dark: var(--secondary);   --white: var(--secondary-ultra-dark); }`
Code language: CSS (css)

The point is that variables have additional superpowers where static values do not.

---

*This documentation was extracted from the database for URLs containing 'automaticcss'*
