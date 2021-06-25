# Change Animation Timing with Keywords

In CSS animations, the `animation-timing-function` property controls how quickly an animated element changes throughout the animation. If the animation is a car moving from point A to point B in a given time (you `animation-duration`), the `animation-timing-function` says how the car accelerates and decelerates throughout the drive.

There are several predefined keywords available for popular options. For example, the default value is `ease`, which starts slow, speeds up in the middle, and then slows down again in the end. Other options include `ease-out`, which is quick in the beginning then slows down, `ease-in`, which is slow in the beginning, then speeds up at the end, or `linear`, which applies a constant animation speed throughout.

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
        .balls {
            border-radius: 50%;
            background: linear-gradient(
                35deg,
                #CCFFFF,
                #FFCCCC
            );
            position: fixed;
            width: 50px;
            height: 50px;
            margin-top: 50px;
            animation-name: bounce;
            animation-duration: 2s;
            animation-iteration-count: infinite;
        }

        #ball1 {
            left: 27%;
            animation-timing-function: linear;
        }

        #ball2 {
            left: 56%;
            animation-timing-function: ease-out;
        }

        @keyframes bounce {
            0% {
                top: 0;
            }
            100% {
                top: 249px;
            }
        }
    </style>
</head>
<body>
    <div class="balls" id="ball1"></div>
    <div class="balls" id="ball2"></div>
</body>
</html>
```

[Applied Visual Design](../applied-visual-design.md) | [Responsive Web Design](../../responsive-web-design.md)