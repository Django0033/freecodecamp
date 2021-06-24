# Make a CSS Heartbeat using an Infinite Animation Count

Here's one more continuous animation example with the `animation-iteration-count` property that uses the heart you designed in a previous challenge.

The one-second-long heartbeat animation consists of two animated pieces. The `heart` element (including the `:before` and `:after` pieces) are animated to change the size using the `transform` property, and the background `div` is animated to change its color using the `background` property.

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
        .back { 
            position: fixed;
            padding: 0;
            margin: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background: white;
            animation-name: backdiv;
            animation-duration: 1s;
            animation-iteration-count: infinite;
        }

        .heart {
            position: absolute;
            margin: auto;
            top: 0;
            right: 0;
            bottom: 0;
            left: 0;
            background-color: pink;
            height: 50px;
            width: 50px;
            transform: rotate(-45deg);
            animation-name: beat;
            animation-duration: 1s;
            animation-iteration-count: infinite;
        }

        .heart::after {
            background-color: pink;
            content: "";
            border-radius: 50%;
            position: absolute;
            width: 50px;
            height: 50px;
            top: 0;
            left: 25px;
        }

        .heart::before {
            background-color: pink;
            content: "";
            border-radius: 50%;
            position: absolute;
            width: 50px;
            height: 50px;
            top: -25px;
            left: 0;
        }

        @keyframes backdiv {
            50% {
                background: #FFE6F2;
            }
        }

        @keyframes beat {
            0% {
                transform: scale(1) rotate(-45deg);
            }
            50% {
                transform: scale(0.6) rotate(-45deg);
            }
        }
    </style>
</head>
<body>
    <div class="back"></div>
    <div class="heart"></div>
</body>
</html>
```

[Applied Visual Design](../applied-visual-design.md) | [Responsive Web Design](../../responsive-web-design.md)
