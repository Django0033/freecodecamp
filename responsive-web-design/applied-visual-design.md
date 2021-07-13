# Applied Visual Design

## Table of Content
<!-- vim-markdown-toc GFM -->

* [Create Visual Balance Using the text-align Property](#create-visual-balance-using-the-text-align-property)
    * [Example](#example)
* [Adjust the Width of an Element Using the width Property](#adjust-the-width-of-an-element-using-the-width-property)
    * [Example](#example-1)
* [Adjust the Height of an Element Using the height Property](#adjust-the-height-of-an-element-using-the-height-property)
    * [Example](#example-2)
* [Use the strong Tag to Make Text Bold](#use-the-strong-tag-to-make-text-bold)
    * [Example](#example-3)
* [Use the u Tag to Underline Text](#use-the-u-tag-to-underline-text)
    * [Example](#example-4)
* [Use the em Tag to Italicize Text](#use-the-em-tag-to-italicize-text)
    * [Example](#example-5)
* [Use the s Tag to Strikethrough Text](#use-the-s-tag-to-strikethrough-text)
    * [Example](#example-6)
* [Create a Horizontal Line Using the hr Element](#create-a-horizontal-line-using-the-hr-element)
    * [Example](#example-7)
* [Adjust the background-color Property of Text](#adjust-the-background-color-property-of-text)
    * [Example](#example-8)
* [Adjust the Size of a Header Versus a Paragraph Tag](#adjust-the-size-of-a-header-versus-a-paragraph-tag)
    * [Example](#example-9)
* [Add a box-shadow to a Card-like Element](#add-a-box-shadow-to-a-card-like-element)
    * [Example](#example-10)
* [Decrease the Opacity of an Element](#decrease-the-opacity-of-an-element)
    * [Example](#example-11)
* [Use the text-transform Property to Make Text Uppercase](#use-the-text-transform-property-to-make-text-uppercase)
    * [Example](#example-12)
* [Set the font-size for Multiple Heading Elements](#set-the-font-size-for-multiple-heading-elements)
    * [Example](#example-13)
* [Set the font-weight for Multiple Heading Elements](#set-the-font-weight-for-multiple-heading-elements)
    * [Example](#example-14)

<!-- vim-markdown-toc -->
## Create Visual Balance Using the text-align Property

This section of the curriculum focuses on Applied Visual Design. The first group of challenges builds on the given card layout to show some core principles.

Text is often a large part of web content. CSS has several options for how to align it with the `text-align` property.

`text-align: justify;` causes all lines of text except the last line to meet the left and right edges of the line box.

`text-align: center;` centers the text.

`text-align: right;` right-aligns the text.

And `text-align: left;` (the default) left-aligns the text.

### Example

```html
<style>
  h4 {
    text-align: center;
  }
  p {
    text-align: justify;
  }
  .links {
    margin-right: 20px;

  }
  .fullCard {
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at Stanford University.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Adjust the Width of an Element Using the width Property

You can specify the width of an element using the `width` property in CSS. Values can be given in relative length units (such as `em`), absolute length units (such as `px`), or as a percentage of its containing parent element. Here's an example that changes the width of an image to 220px:

```css
img {
  width: 220px;
}
```

### Example

```html
<style>
  h4 {
    text-align: center;
  }
  p {
    text-align: justify;
  }
  .links {
    margin-right: 20px;
    text-align: left;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at Stanford University.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```


[Table of Content](#table-of content)

## Adjust the Height of an Element Using the height Property

You can specify the height of an element using the `height` property in CSS, similar to the `width` property. Here's an example that changes the height of an image to 20px:

```css
img {
  height: 20px;
}
```

### Example

```HTML
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    margin-right: 20px;
    text-align: left;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at Stanford University.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Use the strong Tag to Make Text Bold

To make text bold, you can use the `strong` tag. This is often used to draw attention to the text and symbolize that it is important. With the `strong` tag, the browser applies the CSS of `font-weight:bold;` to the element.

### Example

```html
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at <strong>Stanford University</strong>.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Use the u Tag to Underline Text

To underline text, you can use the `u` tag. This is often used to signify that a section of text is imgortant, or something to remember. With the `u` tag, the browser applies the CSS of `text-decoration:underline;` to the element.

### Example

```HTML
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Use the em Tag to Italicize Text

To emphasize text, you can use the `em` tag. This displays text as italicized, as the browser applies the CSS of `font-style: italic; to the element.

### Example

```HTML
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Use the s Tag to Strikethrough Text

To strikethrough text, which is when a horizontal line cuts across the characters, you can use the `s` tag. It shows that a section of text is no longer valid. With the `s` tag, the browser applies the CSS of `text-decoration: line-through;` to the element.

### Example

```html
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4><s>Google</s> Alphabet</h4>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Create a Horizontal Line Using the hr Element

You can use the `hr` tag to add a horizontal line across the width of its containing element. This can be used to define a change in topic or to visually separate groups of content.

### Example

```html
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4><s>Google</s>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Adjust the background-color Property of Text

Instead of adjusting your overall background or the color of the text to make the foreground easily readable, you can add a `background-color` to the element holding the text you want to emphasize. This challenge uses `rgba()` instead of `hex` codel or normal `rgb()`.

> rgba stands for:<br>
	r = red<br>
	g = green<br>
	b = blue<br>
	a = alpha/level of opacity
	
The RGB values can range from 0 to 255. The alpha value can range from 1, which is fully opaque or a solid color, to 0, which is fully tronsparent or clear. `rgba()` is great to use in this case, as it allows you to adjust the opacity. This means you don't have to completely block out the background.

You'll use `background-color: rgba(45, 45, 45, 0.1)` for this challenge. It produces a dark gray color that is nearly transparent given the low opacity value of 0.1.

### Example

```html
<style>
  h4 {
    text-align: center;
    padding: 10px;
    background-color: rgba(45, 45, 45, 0.1);

  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Adjust the Size of a Header Versus a Paragraph Tag

The font size of header tags (`h1` through `h6`) should generally be larger than the font size of paragraph tags. This makes it easier for the user to visually understand the layout and level of importance of everything on the page. You use the `font-size` property to adjust the size of the text in an element.

### Example

```html
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size: 27px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Add a box-shadow to a Card-like Element

The `box-shadow` property applies one or more shadows to an element.

The `box-shadow` property takes values for

- `offset-x` (how far to push the shadow horizontally from tho element),
- `offset-y` (how far to push the shadow vertically from the element),
- `blur-radius`,
- `spread-radius` and
- `color`, in that order.

The `blur-radius` and `spread-radius` values are optional.

Multiple box-shadows can be created by using commas to separate properties of each `box-shadow` element.

Here's an example of the CSS to create multiple shadows with some blur, at mostly-transparent black colors:

```css
box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px rgba(0, 0, 0, 0.23);
```

### Example

```HTML
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size: 27px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  #thumbnail {
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
  }

  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard" id="thumbnail">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr />
      <p>
        <em
          >Google was founded by Larry Page and Sergey Brin while they were
          <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em
        >
      </p>
    </div>
    <div class="cardLinks">
      <a
        href="https://en.wikipedia.org/wiki/Larry_Page"
        target="_blank"
        class="links"
        >Larry Page</a
      ><br /><br />
      <a
        href="https://en.wikipedia.org/wiki/Sergey_Brin"
        target="_blank"
        class="links"
        >Sergey Brin</a
      >
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Decrease the Opacity of an Element

The `opacity` property in CSS is used to adjust the opacity, or conversely, the transparency for an item.

> A value of 1 is opaque, which isn't transparent at all.
> A value of 0.5 is half see-through.
> A value of 0 is completely transparent.

The value given will apply to the entire element, whether that's an image with some transparency, or the foreground and background colors for a block of text.

### Example

```html
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size: 27px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
    opacity: 0.7;
  }
  #thumbnail {
    box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard" id="thumbnail">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Use the text-transform Property to Make Text Uppercase

The `text-transform` property in CSS is used to change the appearance of text. It's a convenient way to make sure text on a webpage appears consistently, without having to change the text content of the actual HTML elements.

The following table shows how the different `text-transform` values change the example text "Transform me".

| Value      | Result         |
| ----------- | ----------- |
| lowercase  | "transform me" |
| uppercase  | "TRANSFORM ME" |
| capitalize | "Transform me" |
| initial    | Use the default value |
| inherit    | Use the `text-transform value from the parent element |
| none       | Default: use the original text |

### Example

```html
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size: 27px;
    text-transform: uppercase;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
    opacity: 0.7;
  }
  #thumbnail {
    box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard" id="thumbnail">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Table of Content](#table-of content)

## Set the font-size for Multiple Heading Elements

The `font-size` property is used to specify how large the text is in a given element. This rule can be used for multiple elements to create visual consistency of text on a page. In this challenge, you'll set the values for all `h1` through `h6` tags to balance the heading sizes.

### Example

```html
<style>
  h1 {
    font-size: 68px;
  }
  h2 {
    font-size: 52px;
  }
  h3 {
    font-size: 40px;
  }
  h4 {
    font-size: 32px;
  }
  h5 {
    font-size: 21px;
  }
  h6 {
    font-size: 14px;
  }

</style>
<h1>This is h1 text</h1>
<h2>This is h2 text</h2>
<h3>This is h3 text</h3>
<h4>This is h4 text</h4>
<h5>This is h5 text</h5>
<h6>This is h6 text</h6>
```

[Table of Content](#table-of content)

## Set the font-weight for Multiple Heading Elements

You set the `font-size` of each heading tag in the last challenge, here you'll adjust the `font-weight`.

The `font-weight` property sets how thick or thin characters are in a section of text.

### Example

```html
<style>
  h1 {
    font-size: 68px;
    font-weight: 800;
  }
  h2 {
    font-size: 52px;
    font-weight: 600;
  }
  h3 {
    font-size: 40px;
    font-weight: 500;
  }
  h4 {
    font-size: 32px;
    font-weight: 400;
  }
  h5 {
    font-size: 21px;
    font-weight: 300;
  }
  h6 {
    font-size: 14px;
    font-weight: 200;
  }
</style>
<h1>This is h1 text</h1>
<h2>This is h2 text</h2>
<h3>This is h3 text</h3>
<h4>This is h4 text</h4>
<h5>This is h5 text</h5>
<h6>This is h6 text</h6>
```

[Table of Content](#table-of content)

* [Set the font-size of Paragraph Text](applied-visual-design/set-the-font-size-of-paragraph-text.md)
* [Set the line-height of Paragraphs](applied-visual-design/set-the-line-height-of-paragraphs.md)
* [Adjust the Hover State of an Anchor Tag](applied-visual-design/adjust-the-hover-state-of-an-anchor-tag.md)
* [Change an Element's Relative Position](applied-visual-design/change-an-elements-relative-position.md)
* [Move a Relative Positioned Element with CSS Offsets](applied-visual-design/move-a-relatively-positioned-element-with-css-offsets.md)
* [Lock an Element to its Parent with Absolute Positioning](applied-visual-design/lock-an-element-to-its-parent-with-absolute-positioning.md)
* [Lock an Elment to the Browser Window with Fixed Positioning](applied-visual-design/lock-an-element-to-the-browser-window-with-fixed-positioning.md)
* [Push Elements Left or Right with the float Property](applied-visual-design/push-elements-left-or-right-with-the-float-property.md)
* [Change the Position of Overlapping Elements with the z-index Property](applied-visual-design/change-the-position-of-overlapping-elements-with-the-z-index-property.md)
* [Center an Element Horizontally Using the margin Property](applied-visual-design/center-an-element-horizontally-using-the-margin-property.md)
* [Learn About Complementary Colors](applied-visual-design/learn-about-complementary-colors.md)
* [Learn About Tertiary Colors](applied-visual-design/learn-about-tertiary-colors.md)
* [Adjust the Color of Various Elements to Complementary Colors](applied-visual-design/adjust-the-color-of-various-element-to-complementary-colors.md)
* [Adjust the Hue of a Color](applied-visual-design/adjust-the-hue-of-a-color.md)
* [Adjust the Tone of a Color](applied-visual-design/adjust-the-tone-of-a-color.md)
* [Create a Gradual CSS Linear Gradient](applied-visual-design/create-a-gradual-css-linear-gradient.md)
* [Use a CSS Linear Gradient to Create a Striped Element](applied-visual-design/use-a-css-linear-gradient-to-create-a-striped-element.md)
* [Create Texture by Adding a Subtle Pattern as a Background Image](applied-visual-design/create-texture-by-adding-a-subtle-pattern-as-a-background-image.md)
* [Use the CSS Transform scale Property to Change the Size of an Element](applied-visual-design/use-the-css-transform-scale-property-to-change-the-size-of-an-element.md)
* [Use the CSS Transform scale Property to Scale an Element on Hover](applied-visual-design/use-the-css-transform-scale-property-to-scale-an-element-on-hover.md)
* [Use the CSS Transform Property skewX to Skew an Element Along the X-Axis](applied-visual-design/use-the-css-transform-property-skewx-to-skew-an-element-along-the-x-axis.md)
* [Use the CSS Transform Property skewY to Skew an Element Along the Y-Axis](applied-visual-design/use-the-css-transform-property-skewy-to-skew-an-element-along-the-y-axis.md)
* [Create a Graphic Using CSS](applied-visual-design/create-a-graphic-using-css.md)
* [Create a More Complex Shape Using CSS and HTML](applied-visual-design/create-a-more-complex-shape-using-css-and-html.md)
* [Learn How the CSS @keyframes and animation Properties Work](applied-visual-design/learn-how-the-css-keyframes-and-animation-properties-work.md)
* [Use CSS Animation to Change the Hover State of a Button](applied-visual-design/use-css-animation-to-change-the-hover-state-of-a-button.md)
* [Modify Fill Mode of an Animation](applied-visual-design/modify-fill-mode-of-an-animation.md)
* [Create Movement Using CSS Animation](create-applied-visual-design/create-movement-using-css-animation.md)
* [Create Visual Direction by Fading an Element from Left to Right](applied-visual-design/create-visual-direction-by-fading-an-element-from-left-to-right.md)
* [Animate Elements Continually Using an Infinite Animation Count](applied-visual-design/animate-elements-continually-using-an-infinite-animation-count.md)
* [Make a CSS Heartbeat using an Infinite Animation Count](applied-visual-design/make-a-css-heartbeat-using-an-infinite-animation-count.md)
* [Animate Elements at Variable Rates](applied-visual-design/animate-elements-at-variable-rates.md)
* [Animate Multiple Elements at Variable Rates](applied-visual-design/animate-multiple-elements-at-variable-rates.md)
* [Change Animation Timing with Keywords](applied-visual-design/change-animation-timing-with-keywords.md)
* [Learn How Bezier Curves Work](./applied-visual-design/learn-how-bezier-curves-work.md)
* [Use a Bezier Curve to Move a Graphic](./applied-visual-design/use-a-bezier-curve-to-move-a-graphic.md)
* [Make Motion More Natural Using a Bezier Curve](./applied-visual-design/make-motion-more-natural-using-a-bezier-curve.md)

[Responsive Web Design](/responsive-web-design.md)
