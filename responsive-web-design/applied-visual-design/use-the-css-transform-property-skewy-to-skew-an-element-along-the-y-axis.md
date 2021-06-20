# Use the CSS Transform Property skewY to Skew an Element Along the Y-Axis

Given that the `skewX()` function skews the selected element along the X-axis by a given degree, it is no surprise that the `skewY()` property skews an element along the Y (vertical) axis.

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

        div {
            width: 70%;
            height: 100px;
            margin: 50px auto;
        }

        #top {
            background-color: red;
            transform: skewY(-10deg);
        }

        #bottom {
            background-color: blue;
            transform: skewX(24deg);
        }

    </style>
</head>
<body>

    <div id="top"></div>
    <div id="bottom"></div>
    
</body>
</html>
```

[Applied Visual Design](/responsive-web-design/applied-visual-design.md) | [Responsive Web Design](/responsive-web-design.md)
