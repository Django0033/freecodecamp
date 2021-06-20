# Override Styles in Subsequent CSS

Our `pink-text` class overrode our `body` element's CSS declaration!

We just proved that our classes will override the `body` element's CSS. So the next logical question is, what can we do to override our `pink-text` class?

## Example

```html
<style>
  body {
    background-color: black;
    font-family: monospace;
    color: green;
  }
  .pink-text {
    color: pink;
  }

  .blue-text {
    color: blue;
  }
</style>
<h1 class="pink-text blue-text">Hello World!</h1>
```

[Basic CSS](../basic-css.md) | [Responsive Web Design](../../responsive-web-design.md)
