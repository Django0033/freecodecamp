# Adjust the Hue of a Colors

Colors have several characteristics including hue, saturation, and lightness. CSS3 introduced the `hsl()` property as an alternative way to pick a color by directly stating these characteristics.

**Hue** is what people generally think of as 'color'. If you picture a spectrum of colors starting with red on the left, moving through green in the middle, and blue on right, the hue is where a color fits along this line. In `hsl()`, hue uses a color wheel concept instead of the spectrum, where the angle of the color on the circle is given as a value between 0 and 360.

**Saturation** is the amount of gray in a color. A fully saturated color has no gray in it, and a minimally saturated color is almost completely gray. This is given as a percentage with 100% being fully saturated.

**Lightness** is the amount of white or black in a color. A percentage is given ranging from 0% (black) to 100% (white), where 50% is the normal color.

Here are few examples of using `hsl()` with fully-saturated, normal lightness colors:

| Color | HSL |
| --- | --- |
| Red | hsl(0, 100%, 50%) |
| Yellow | hsl(60, 100%, 50%) |
| Green | hsl(120, 100%, 50%) |
| Cyan | hsl(180, 100%, 50%) |
| Blue | hsl(240, 100%, 50%) |
| Magenta | hsl(300, 100%, 50%) |

## Example

```html
<style>
  body {
    background-color: #FFFFFF;
  }

  .green {
    background-color: hsl(120, 100%, 50%);
  }

  .cyan {
    background-color: hsl(180, 100%, 50%);
  }

  .blue {
    background-color: hsl(240, 100%, 50%);
  }

  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>

<div class="green"></div>
<div class="cyan"></div>
<div class="blue"></div>
```

[Applied Visual Design](../applied-visual-design.md) | [Responsive Web Design](../../responsive-web-design.md)
