# Add Different Padding to Each Side of an Element

Sometimes you will want to customize an element so that it has different amounts of `padding` on each of its sides.

CSS allows you to control the `padding` of all four individual sides of an element with the `padding-top`, `padding-right`, `padding-bottom`, and `padding-left` properties.

## Example

```html
<style>
  .injected-text {
    margin-bottom: -25px;
    text-align: center;
  }

  .box {
    border-style: solid;
    border-color: black;
    border-width: 5px;
    text-align: center;
  }

  .yellow-box {
    background-color: yellow;
    padding: 10px;
  }

  .red-box {
    background-color: crimson;
    color: #fff;
    padding-top: 40px;
    padding-right: 20px;
    padding-bottom: 20px;
    padding-left: 40px;
  }

  .blue-box {
    background-color: blue;
    color: #fff;
    padding-top: 40px;
    padding-left: 40px;
    padding-right: 20px;
    padding-bottom: 20px;
  }
</style>
<h5 class="injected-text">margin</h5>

<div class="box yellow-box">
  <h5 class="box red-box">padding</h5>
  <h5 class="box blue-box">padding</h5>
</div>
```

[Basic CSS](../basic-css.md) | [Responsive Web Design](../../responsive-web-design.md)
