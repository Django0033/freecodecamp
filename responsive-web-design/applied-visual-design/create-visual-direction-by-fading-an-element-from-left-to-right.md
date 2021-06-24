# Create Visual Direction by Fading an Element from Left to Right

For this challenge, you'll change the `opacity` of an animated element on it gradually fades as it reaches the right side of the screen.

In the displayed animation, the round element with the gradient background moves to the right by the 50% mark of the animation per the `@keyframes` rule.

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
        
        #ball {
            width: 70px;
            height: 70px;
            margin: 50px auto;
            position: fixed;
            left: 20%;
            border-radius: 50%;
            background-color: linear-gradient(
                35deg,
                #CCFFFF,
                #FFCCCC
            );
            animation-name: fade;
            animation-duration: 3s;
        }

        @keyframes fade {
            50% {
                left: 60%;
                opacity: 0.1;
            }
        }
    </style>
</head>
<body>
    <div id="ball"></div> 
</body>
</html>
```

[Applied Visual Design](/responsive-web-design/applied-visual-design.md) | [Responsive Web Design](/responsive-web-design.md)
