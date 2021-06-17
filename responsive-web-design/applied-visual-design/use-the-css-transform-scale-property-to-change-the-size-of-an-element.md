# Use the CSS Transform scale Property to Change the Size of an Element

To change the scale of an element, CSS has the `transform` property, along with its `scale()` function. The Following code example doubles the size of all the paragraph elements on the page:

```css
p {
    transform: scale(2);
}
```

## Example

```html
<style>
  .ball {
    width: 40px;
    height: 40px;
    margin: 50 auto;
    position: fixed;
    background: linear-gradient(
      35deg,
      #ccffff,
      #ffcccc
    );
    border-radius: 50%;
  }
  #ball1 {
    left: 20%;
  }
  #ball2 {
    left: 65%;
    transform: scale(1.5);
  }


</style>

<div class="ball" id= "ball1"></div>
<div class="ball" id= "ball2"></div>
```

[Applied Visual Design](../applied-visual-design.md) | [Responsive Web Design](../../responsive-web-design.md)
