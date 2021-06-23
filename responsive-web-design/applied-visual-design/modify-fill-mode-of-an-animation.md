# Modify Fill Mode of an Animation

That's great, but it doesn't work right yet. Notice how the animation resets after `500ms` has passed, causing the button to revert to the original color. You want the button to stay highlighted.

This can be done by setting the `animation-fill-mode` property to `forwards`. The `animation-fill-mode` specifies the style applied to an element when the animation has finished. You can set it like so:

```CSS
animation-fill-mode: forwards;
```

## Example

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        button {
            border-radius: 5px;
            color: white;
            background-color: #0F5897;
            padding: 5px 10px 8px 10px;
        }

        button:hover {
            animation-name: background-color;
            animation-duration: 500ms;
            animation-fill-mode: forwards;
        }

        @keyframes background-color {
            100% {
                background-color: #4791D0;
            }
        }
    </style>
</head>
<body>
    <button>Register</button> 
</body>
</html>
```

[Applied Visual Design](../applied-visual-design.md) | [Responsive Web Design](../../responsive-web-design.md)
