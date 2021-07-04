# Add a Text Alternative to Images for Visually Impaired Accessibility

You've likely seen an `alt` attribute on an `img` tag in other challenges. `alt` text describes the image's content and provides a text-alternative for it. An `alt` attribute helps in cases where the image fails to load or can't be seen by a user. Search engines also use it to understand what an image contains to include it in search results. Here's an example:

```HTML
<img src="importantLogo.jpeg" alt="Company logo">
```

People with visual impairments rely on screen readers to convert web content to an audio interface. They won't get information if it's only presented visually. For images, screen readers can access the `alt` attribute and read its contents to deliver key information.

Good `alt` text provides the reader a brief description of the image. You should always include an `alt` attribute on your images. Per HTML5 specification, this is now considered mandatory.

## Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>
            Add a Text Alternative to Images for Visually Impaired Accessibility
        </title>
    </head>
    <body>
        <img src="doingKarateWow.jpeg" alt="Camper Cat doing karate" />
    </body>
</html>
```

[Applied Accessibility](../applied-accessibility.md) | [Responsive Web Design](../../responsive-web-design.md)
