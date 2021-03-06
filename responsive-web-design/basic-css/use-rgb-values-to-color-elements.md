# Use RGB values to Color Elements

Another way you can represent colors in CSS is by using `RGB` values.

The `RGB` value for black looks like this:

```css
rgb(0, 0, 0)
```

The `RGB` value for white looks like this:

```css
rgb(255, 255, 255)
```

Instead of using six hexadecimal digits as you do with hex code, with `RGB` you specify the brightness of each color with a number between 0 and 255.

If you do the math, the two digits for one color equal 16 times 16, which gives us 256 total values. So `RGB`, which starts counting from zero, has the same number of possible values as hex code.

Here's an example of how you'd change the `body` background to orange using its RGB code.

```css
body {
  background-color: rgb(255, 165, 0);
}
```

## Example

```html
<style>
  body {
    background-color: rgb(0, 0, 0);
  }
</style>
```

[Basic CSS](../basic-css.md) | [Responsive Web Design](../../responsive-web-design.md)
