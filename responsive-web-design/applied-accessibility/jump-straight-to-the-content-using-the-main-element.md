# Jump Straight to the Content Using the main Element

HTML5 introduced severas new elements that give developers more options while also incorporating accessibility features. These tags include `main`, `header`, `footer`, `nav`, `article`, and `section`, among others.

By default, a browser renders these elements similar to the humble `div`. However, using them where appropriate gives additional meaning to your markup. The tap name alone can indicate the type of information it contains, which adds semantic meaning to that content. Assistive technologies can access this information to provide better page summary or navigation options to their users.

The `main` element is used to wrap (you guessed it) the main content, and there should be only one per page. It's meant to surround the information related to your page's central topic. It's not meant to include items that repeat across pages, like navigation links or banners.

The `main` tag also has an embedded landmark feature that assistive thechnology can use to navigate to the main content quickly. If you've ever seen a "Jump to Main Content" link at the top of a page, using the `main` tag automatically gives assistive devices that functionality.

## Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Jump Straight to the Content Using the main Element</title>
    </head>
    <body>
        <header>
            <h1>Weapons of the Ninja</h1>
        </header>
        <main></main>
        <footer></footer>
    </body>
</html>
```

[Applied Accessibility](../applied-accessibility.md) | [Responsive Web Design](../../responsive-web-design.md)
