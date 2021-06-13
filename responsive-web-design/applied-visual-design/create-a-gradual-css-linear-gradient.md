# Create a Gradual CSS linear Gradient

Applying a color on HTML elements is not limited to one flat hue. CSS provides the ability to use color transitions, otherwise known as gradients, on elements. This is accessed through the `background` property's `linear-gradient()` function. Here is the general syntax:

```CSS
background: linear-gradient(gradient_direction, color 1, color 2, color 3,...);
```

The first argument specifies the direction from which color transition starts-it can be stated as a degree, where `90deg` makes a horizontal gradient (from left to right) and `45deg` makes a diagonal gradient (from bottom left to top right). The following arguments specify the order of colors used in the gradient.

```css
background: linear-gradient(90deg, red, yellow, rgb(204, 204, 255));
```

## Example

```html
<style>
  div {
    border-radius: 20px;
    width: 70%;
    height: 400px;
    margin: 50px auto;
    background: linear-gradient(35deg, #CCFFFF, #FFCCCC)
  }

</style>

<div></div>
```

[Applied Visual Design](/responsive-web-design/applied-visual-design.md) | [Responsive Web Design](/responsive-web-design.md)
