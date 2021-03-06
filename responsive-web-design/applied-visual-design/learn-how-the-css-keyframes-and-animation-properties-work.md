# Learn How the CSS @keyframes and animation Properties Work

To animate an element, you need to know about the animation properties and the `@keyframes` rule. The animation properties control how the animation should behave and the `@keyframes` rule controls what happens during that animation. There are eight animation properties in total. This challenge will keep it simple and cover the two most important ones first:

`animation-name` sets the name of the animation, which is later used by `@keyframes` to tell CSS which rules go with which animations.

`animation-duration` sets the length of time for the animation.

`@keyframes` is how to specify exactly what happens within the animation over the duration. This is done by giving CSS properties for specific "frames" during the animation, with percentages ranging from 0% to 100%. If you compare this to a movie, the CSS properties for 0% is how the element displays in the opening scene. The CSS properties for 100% is how the element appears at the end, right before the credits roll. Then CSS applies the magic to transition the element over the given duration to act out the scene. Here's an example to illustrate the usage of `@keyframes` and the animation properties:

```CSS
#anim {
    animation-name: colorful;
    animation-duration: 3s;
}

@keyframes colorful {
    0% {
        background-color: blue;
    }
    100% {
        background-color: yellow;
    }
}
```

For the element with the `anim` id, the code snippet above sets the `animation-name` to `colorful` and sets the `animation-duration` to 3 seconds. Then the `@keyframes` rule links to the animation properties with the name `colorful`. It sets the color to blue at the beginning of the animation (0%) which will transition to yellow by the end of the animation (100%). You aren't limited to only beginning-end transitions, you can set properties for the element for any percentage between 0% and 100%.

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
            height: 40px;
            width: 70%;
            background: black;
            margin: 50px auto;
            border-radius: 5px;
        }
        #rect {
            animation-name: rainbow;
            animation-duration: 4s;
        }
        @keyframes rainbow {
            0% {
                background-color: blue;
            }
            50% {
                background-color: green;
            }
            100% {
                background-color: yellow;
            }
        }
    </style>
</head>
<body>
    <div id="rect"></div>
</body>
</html>
```

[Applied Visual Design](/responsive-web-design/applied-visual-design.md) | [Responsive Web Design](/responsive-web-design.md)
