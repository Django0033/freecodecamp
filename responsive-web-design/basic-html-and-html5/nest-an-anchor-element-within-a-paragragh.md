# Nest an Anchor Element within a Paragraph

You can nest links within other text elements.

```html
<p>
  Here's a <a target="_blank" href="https://www.freecodecamp.org"> link to www.freecodecamp.org</a> for you to follow.
</p>
```

Let's break down the example. Normal text is wrapped in the p element:

```html
<p> Here's a ... for you to follow. </p>
```

Next is the anchor element `<a>` (which requires a closing tag `</a>`):

```html
<a> ... </a>
```

`target` is an anchor tag attribute that specifies where to open the link. The value `_blank` specifies to open the link in a new tab. The `href` is an anchor tag attribute that contains the URL address of the link:

```html
<a href="https://www.freecodecamp.org" target="_blank"> ... </a>
```

The text, `link to www.freecodecamp.org`, within the a element is called anchor text, and will display the link to click:

```html
<a href=" ... " target="...">link to freecodecamp.org</a>
```

The final output of the example will look like this:

Here's a link to www.freecodecamp.org for you to follow.

## Example

```html
<h2>CatPhotoApp</h2>
<main>

  <p>
    View more <a href="https://www.freecatphotoapp.com">cat photos</a>
  </p>

  <img src="https://www.bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back.">

  <p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
  <p>Purr jump eat the grass rip the couch scratched sunbathe, shed everywhere rip the couch sleep in the sink fluffy fur catnip scratched.</p>
  
</main>
```

[Basic HTML and HTML5](../basic-html-and-html5.md) | [Responsive Web Design](/responsive-web-design.md)