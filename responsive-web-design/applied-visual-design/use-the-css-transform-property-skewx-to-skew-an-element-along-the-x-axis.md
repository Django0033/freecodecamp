# Use the CSS Transform Property skewX to Skew an Element Along the X-Axis

The next function of the `transform` property is `skewX()`, which skews the selected element along its X (horizontal) axis by a given degree.

The following code skews the paragraph element by -32 degrees along the X-axis.

```CSS
p {
    transform: skewX(-32deg);
}
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
        div {
            width: 70%;
            height: 100px;
            margin: 50px auto;
        }
        #top {
            background-color: red;
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
