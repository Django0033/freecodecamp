# Basic HTML and HTML5

## Table of Contents

* [Table of Contents](#table-of-contents)
* [Say Hello to HTML Elements](#say-hello-to-html-elements)
* [Headline with the h2 Element](#headline-with-the-h2-element)
* [Inform with the Paragraph Element](#inform-with-the-paragraph-element)
* [Fill in the Blank with Placeholder TextPassed](#fill-in-the-blank-with-placeholder-textpassed)
* [Uncomment HTML](#uncomment-html)
* [Comment out HTMLPassed](#comment-out-htmlpassed)
* [Delete HTML Elements](#delete-html-elements)
* [Introduction to HTML5 Elements](#introduction-to-html5-elements)
* [Add Images to Your Website](#add-images-to-your-website)

- [Link to External Pages with Anchor Elements](basic-html-and-html5/link-to-external-pages-with-anchor-elements.md)
- [Link to Internal Sections of a Page with Anchor Elements](basic-html-and-html5/link-to-internal-sections-of-a-page-with-anchor-elements.md)
- [Nest an Anchor Element within a Paragraph](basic-html-and-html5/nest-an-anchor-element-within-a-paragragh.md)
- [Make Dead Links Using the Hash Symbol](basic-html-and-html5/make-dead-links-using-the-hash-symbol.md)
- [Turn an Image into a Link](basic-html-and-html5/turn-an-image-into-a-link.md)
- [Create a Bulleted Unordered List](basic-html-and-html5/create-a-bulleted-unordered-list.md)
- [Create an Ordered List](basic-html-and-html5/create-an-ordered-list.md)
- [Create a Text Field](basic-html-and-html5/create-a-text-field.md)
- [Add Placeholder Text to a Text Field](basic-html-and-html5/add-placeholder-text-to-a-text-field.md)
- [Create a Form Element](basic-html-and-html5/create-a-form-element.md)
- [Add a Submit Button to a Form](basic-html-and-html5/add-a-submit-button-to-a-form.md)
- [Use HTML5 to Require a Field](basic-html-and-html5/use-html5-to-require-a-field.md)
- [Create a Set of Radio Buttons](basic-html-and-html5/create-a-set-of-radio-buttons.md)
- [Create a Set of Checkboxes](basic-html-and-html5/create-a-set-of-checkboxes.md)
- [Use the Value attribute with Radio Buttons and Checkboxes](basic-html-and-html5/use-the-value-attibute-with-radio-buttons-and-checkboxes.md)
- [Nest Many Elements within a Single div Element](basic-html-and-html5/nest-many-elements-within-a-single-div-element.md)
- [Declare the Doctype of an HTML Document](basic-html-and-html5/declare-the-doctype-of-an-html-document.md)
- [Define the Head and Body of an HTML Document](basic-html-and-html5/define-the-head-and-body-of-an-html-document.md)

[Responsive Web Design](/responsive-web-design.md)

## Say Hello to HTML Elements

Welcome to freeCodeCamp's HTML coding challenges. These will walk you through
web development step-by-step.

First, you'll start by building a simple web page using HTML. You can edit code
in your code editor, which is embedded into this web page.

Do you see the code in your code editor that says `<h1>Hello</h1>`? That's an
HTML element.

Most HTML elements have an opening tag and a closing tag.

Opening tags look like this:

```html
<h1>
```

Closing tags look like this:

```html
</h1>
```

The only difference between opening and closing tags is the forward slash after
the opening bracket of a closing tag.

Each challenge has tests you can run at any time by clicking the "Run tests"
button. When you pass all tests, you'll be prompted to submit your solution and
go to the next coding challenge.

### Example

```html
<h1>Hello World</h1>
```

[Table of Contents](#table-of-contents)

## Headline with the h2 Element

Over the next few lessons, we'll build an HTML5 cat photo web app
piece-by-piece.

The `h2` element you will be adding in this step will add a level two heading
to the web page.

This element tells the browser about the structure of your website. h1 elements
are often used for main headings, while `h2` elements are generally used for
subheadings. There are also `h3`, `h4`, `h5` and `h6` elements to indicate
different levels of subheadings.

### Example

```html
<h1>Hello World</h1>
<h2>CatPhotoApp</h2>
```

[Table of Contents](#table-of-contents)

## Inform with the Paragraph Element

`p` elements are the preferred element for paragraph text on websites. `p` is
short for "paragraph".

You can create a paragraph element like this:

```html
<p>I'm a p tag!</p>
```

### Example

```html
<h1>Hello World</h1>
<h2>CatPhotoApp</h2>
<p>Hello Paragraph</p>
```

[Table of Contents](#table-of-contents)

## Fill in the Blank with Placeholder TextPassed

Web developers traditionally use *lorem ipsum* text as placeholder text. The
lorem ipsum text is randomly scraped from a famous passage by Cicero of Ancient
Rome.

Lorem ipsum text has been used as placeholder text by typesetters since the
16th century, and this tradition continues on the web.

Well, 5 centuries is long enough. Since we're building a CatPhotoApp, let's use
something called "kitty ipsum" text.

### Example

```html
<h1>Hello World</h1>

<h2>CatPhotoApp</h2>

<p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching
attack your ankles chase the red dot, hairball run catnip eat the grass
sniff.</p> ```

[Table of Contents](#table-of-contents)

## Uncomment HTML

Commenting is a way that you can leave comments for other developers within
your code without affecting the resulting output that is displayed to the end
user.

Commenting is also a convenient way to make code inactive without having to
delete it entirely.

Comments in HTML start with `<!--` and end with a `-->`

[Table of Contents](#table-of-contents)

## Comment out HTMLPassed

Remember that in order to start a comment, you need to use `<!--` and to end a
comment, you need to use `-->`

Here you'll need to end the comment before your `h2` element begins.

### Example

```html
<!--
<h1>Hello World</h1>
-->
<h2>CatPhotoApp</h2>
<!--
<p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
-->
```

[Table of Contents](#table-of-contents)

## Delete HTML Elements

Our phone doesn't have much vertical space.

Let's remove the unnecessary elements so we can start building our CatPhotoApp.

### Example

```html
<h2>CatPhotoApp</h2>

<p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching
attack your ankles chase the red dot, hairball run catnip eat the grass
sniff.</p> ```

[Table of Contents](#table-of-contents)

## Introduction to HTML5 Elements

HTML5 introduces more descriptive HTML tags. These include `main`, `header`,
`footer`, `nav`, `video`, `article`, `section` and others.

These tags give a descriptive structure to your HTML, make your HTML easier to
read, and help with Search Engine Optimization (SEO) and accessibility. The
main HTML5 tag helps search engines and other developers find the `main`
content of your page.

Example usage, a `main` element with two child elements nested inside it:

```html
<main> 
  <h1>Hello World</h1>
  <p>Hello Paragraph</p>
</main>
```

Note: Many of the new HTML5 tags and their benefits are covered in the Applied
Accessibility section.

### Example

```html
<h2>CatPhotoApp</h2>

<main>

  <p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching
  attack your ankles chase the red dot, hairball run catnip eat the grass
  sniff.</p> <p>Purr jump eat the grass rip the couch scratched sunbathe, shed
  everywhere rip the couch sleep in the sink fluffy fur catnip scratched.</p>

</main>
```

[Table of Contents](#table-of-contents)

## Add Images to Your Website

You can add images to your website by using the `img` element, and point to a
specific image's URL using the `src` attribute.

An example of this would be:

```html
<img src="https://www.freecatphotoapp.com/your-image.jpg">
```

Note that `img` elements are self-closing.

All `img` elements must have an `alt` attribute. The text inside an `alt`
attribute is used for screen readers to improve accessibility and is displayed
if the image fails to load.

Note: If the image is purely decorative, using an empty `alt` attribute is a
best practice.

Ideally the `alt` attribute should not contain special characters unless needed.

Let's add an `alt` attribute to our `img` example above:

```html
<img src="https://www.freecatphotoapp.com/your-image.jpg" alt="A business cat wearing a necktie.">
```

### Example

```html
<h2>CatPhotoApp</h2>
<main>
<img src="https://www.bit.ly/fcc-relaxing-cat" alt="A cat laying down on his back."

  <p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching
  attack your ankles chase the red dot, hairball run catnip eat the grass
  sniff.</p> <p>Purr jump eat the grass rip the couch scratched sunbathe, shed
  everywhere rip the couch sleep in the sink fluffy fur catnip scratched.</p>
</main>
```

[Table of Contents](#table-of-contents)
