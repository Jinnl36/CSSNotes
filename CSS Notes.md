## Different Styles
### Inline Styles
 - Using inline styles means adding styles directly to individual HTML elements. These are perfect for quick styling fixes, but can lead to code clutter and reduced maintainability
 - Inline styles are applied directly to individual elements, like coloring a specific word in a sentence
```html
<p style = "color: blue;">Hello, CSS!</p>
```
### Internal Styles
 - Internal styles refers to using a tag called `<style>` placed within the `<head>` section of your HTML
 - It lets you embed CSS rules directly within the HTML document. This can be particularly useful when you are dealing with a single-page project. A example with the structure can be:
```html
<head>
  <style>
    p {
      color: red;
    }
  </style>
</head>

<body>
  <p>Hello, CSS!</p>
</body>
```

### External Stylesheets
 -  Using external stylesheets means creating separate CSS files (.css) that you link to your HTML. This method keeps your styles organized and consistent across multiple pages. It's a popular choice for larger projects.
 -  An example of utilizing a .css file with HTML would be:
```html
<link rel="stylesheet" type="text/css" href="styles.css">
```
 -  This refers to the file styles.css, a example of a css file may be:
```css
p {
  color: green;
}
```

## Pros and Cons
### Inline Styles
#### Advantages
 - Immediate Application - inline styles are applied directly to specific HTML elements. This means that change takes place instantly, making them suitable for quick frontend adjustments
 - Specificity - inline styles have high specificity, meaning they can easily override other styles, such as those from external stylesheets
 - One-off Customization - When you need to style a single element uniquely, inline styles offer a convenient solution.
#### Disadvantages
 - Lack of Separation - inline styles mix content with presentation， making it harder to maintain and troubleshoot your styles as your project grows.
 - Repetition - if you have multiple elements that reqire the same styling, you'll need to duplicate the same inline style for each one
 - Priority Issues - Inline styles can become cumbersome when dealing with specificity conflicts, leading to unexpected results.

