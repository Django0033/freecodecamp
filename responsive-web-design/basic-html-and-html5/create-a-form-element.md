# Create a Form Element

You can build web forms that actually submit data to a server using nothing more than pure HTML. You can do this by specifying an `action` attribute on your form element.

For example:

```html
<form action="/url-where-you-want-to-submit-form-data">
  <input>
</form>
```

## Example

```html
<h2>CatPhotoApp</h2>
<main>
  <p>Click here to view more <a href="#">cat photos</a>.</p>

  <a href="#"><img src="https://www.bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="https://www.freecatphotoapp.com/submit-cat-photo">
    <input type="text" placeholder="cat photo URL">
  </form>
</main>
```

[Basic HTML and HTML5](./basic-html-and-html5.md) | [Responsive Web Design](/responsive-web-design/responsive-web-design.md)