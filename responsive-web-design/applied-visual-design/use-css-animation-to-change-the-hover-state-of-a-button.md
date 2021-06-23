# Use CSS Animation to Change the Hover State of a Button

You can use CSS `@keyframes` to change the color of a button in its hover state.

Here's an example of changing the width of an image on hover:

```HTML
<style>
    img:hover {
        animation-name: width;
        animation-duration: 500ms;
    }

    @keyframes width {
        100% {
            width: 40px;
        }
    }
    </style>

    <img src="https://bit.ly/smallgooglelogo" alt="Google's Logo" />
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
        }

        @keyframes background-color {
            100% { 
                background-color: #4791d0;
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
