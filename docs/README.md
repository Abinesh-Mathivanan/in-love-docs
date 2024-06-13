# Introduction

  <span style='color:green; font-weight:bold;'>In-love.js</span>, a lightweight JavaScript library that adds delightful interactive animations to your web pages, inspired by the expression of love! With in-love.js, you can easily create mesmerizing effects like typewriter text animations, heart-shaped blooms, and sparkling cursor trails etc.., adding a touch of romance and magic to your website.

> Impress your CS crush the way nobody had done before.

<br>

# Features

List of available animations <span style='color:green; font-weight:bold;'>in-love.js</span>.

<span style='font-weight:bold;' > Falling Sakura Petals: </span>Simulates gentle falling cherry blossom petals, evoking tranquility and romance with customizable parameters.

<span style='font-weight:bold;' > Fade Message: </span>Subtle message or notification display with CSS transitions, offering non-intrusive communication to users.

<span style='font-weight:bold;' > Pulsing Heart: </span> Dynamic animation of a pulsating heart symbol, adding emotional depth to the user experience.

<span style='font-weight:bold;' > Falling Hearts: </span> Romantic ambiance creation with gracefully falling heart icons, customizable for personalized immersion.

<span style='font-weight:bold;' > Typewriter Effect: </span> Dynamic rendering of text content with a captivating animation, incrementally displaying characters for an engaging user experience.

<span style='font-weight:bold;' > Heart Bloom Animation: </span> Generates animated heart-shaped blooms using vector calculations and rendering techniques, creating visually stunning displays symbolizing love and romance.

<span style='font-weight:bold;' > Sparkle Cursor Animation: </span>Mesmerizing sparkle effect with shimmering particles that fade over time, enhancing the ambiance of HTML elements.


<br>

# Usage

## Installation

You can install `in-love.js` via npm. Run the following command in your terminal:

```bash
npm i in-love.js
```

or you can also download the `in-love.js` library from the [official repository](https://github.com/Abinesh-Mathivanan/in-love.js).


## Implement Animations

Let's say that you have an existing HTML file with the below template.

```HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./vendor/in-love.css">
</head>
<body>
    <div> <!-- Your body content here --> </div>
    <script src="./dist/in-love.js"></script>
</body>
</html>

```

The path of the `JS` and `CSS` files might differ based on the way you install the library.

Make sure you have the library files on path, because the `JS` heavily utilizes `CSS` components and only use the pre-defined identifiers and attributes as explained below.

### Falling Sakura Petals

To implement the sakura petal animation, we define the following structure:

```HTML

<div id="sakura-petal" fall-speed="2" max-size="14" min-size="10" delay="300">
  <!-- Your body content here -->
</div>

```

`id="sakura-petal"`: This unique identifier is used to target the element where the sakura petals animation will be applied.

`fall-speed="2"`: This attribute controls the falling speed of the sakura petals. The value "2" indicates a moderate falling speed. Adjust this value as needed to change the speed. Lower the spped, faster the petal
falls.

`max-size="14"`: Specifies the maximum size of the sakura petals in pixels. Larger values will result in bigger petals.

`min-size="10"`: Sets the minimum size of the sakura petals in pixels. Smaller values will produce smaller petals.

`delay="300"`: Defines the delay (in milliseconds) before the sakura petals animation starts after the page loads. A delay of "300" milliseconds is provided in this example. Adjust as necessary to control the timing of the animation.

> Derived from the famous [sakura.js repo](https://github.com/jhammann/sakura).
I added some functionalities that allows the user to control fall-speed, max-size, min-size and delay rate.


### Fade Message
To utilize the fading messages feature, adhere to the following HTML structure:

```HTML

<div class="fading-messages-container" fade-repeat="true" repeat-speed="2000">
    <div class="fading-message">Message 1</div>
    <div class="fading-message">Message 2</div>
    <div class="fading-message">Message 3</div>
</div>

```

`fading-messages-container`: This class serves as a container for the fading messages. Each message resides within this container.

`fade-repeat="true"`: The fade-repeat attribute is set to "true" to enable continuous message fading. When enabled, the messages will fade in and out repeatedly.

`repeat-speed="2000"`: This attribute specifies the interval (in milliseconds) between message fades. In this example, messages will fade in and out every 2000 milliseconds (2 seconds). Adjust this value as needed for your desired timing.

`fading-message`: This class is applied to each individual message element within the container. It signifies that the text content of these elements should support fading messages.

You could implement this feature in any kind of text or container element by calling the respective class
attributes.

### Pulsing Heart

To implement pulsing heart animation, we define the following structure:

```HTML

<div id="pulsingheart" class="pulsingheart">
  <!-- Your body content here -->
</div>

```

`id="pulsingheart"`: This unique identifier is used to target the element where the pulsing heart animation will be applied.

`class="pulsingheart"`: The CSS class "pulsingheart" is applied to the element to style it according to the pulsing heart animation.

### Falling Hearts

To implement the falling heart animation you could modify the HTML to:

```HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./vendor/in-love.css">
</head>
<body>
    <div id="fallinghearts" heart-color="yellow"> </div>
    <script src="./dist/in-love.js"></script>
</body>
</html>

```

The `fallinghearts` attribute serves as an identifier that the JavaScript script utilizes to activate the falling hearts feature. When the script runs, it searches for an HTML element with the ID (`fallinghearts`) and applies the falling hearts animation to it based on the provided configuration attributes.

 The `heart-color` attribute in the fallinghearts element specifies the color of the falling hearts in the animation. By setting it to "yellow", you customize the appearance of the hearts, making them yellow. This feature supports nine different colorations such as (Red, Pink, Purple, Orange, Yellow, Black, White, Blue, Green).

### Typewriter Animation

To implement the falling heart animation, we could modify the HTML to:

```HTML

<div id="typewriter" love-text="true" text-speed="100" text-font-family="Courier New" text-font-size="16px" text-color="#000000">
  Your text goes here...
</div>

```

`id="typewriter"`: This unique identifier is used to target the element where the typewriter animation will be applied.

`love-text="true"`: This attribute specifies that the text content inside the element should be animated as if it's being typed by a typewriter.

`text-speed="100"`: This attribute sets the speed of the typewriter animation, where 100 represents 100 milliseconds delay between each character being typed.

`text-font-family="Courier New"`: This attribute sets the font family for the typewriter text.

`text-font-size="16px"`: This attribute sets the font size for the typewriter text.

`text-color="#000000"`: This attribute sets the color of the typewriter text to black. You can customize it by providing a different color code.

### Heart Bloom Animation

To implement the Heart Bloom animation, we could modify the HTML to:

```HTML

<script type="text/javascript" src="./vendor/jquery.js"></script>

<div id="loveHeart">
    <canvas id="heartbloom" width="670" height="625"></canvas>
</div>
<script type="text/javascript">
    var offsetX = $("#loveHeart").width() / 2;
    var offsetY = $("#loveHeart").height() / 2 - 55;
    setTimeout(function () {
        startHeartAnimation();
    }, 5000);
</script>

```

`id="loveHeart"`: The id loveHeart is used to contain the animated heart graphic as to be defines with an `div` container.

`id="heartbloom"`: The id heartbloom is used to draw the heart graphic animation with in a `canvas` or a `div` container.

The Javascript used in this HTML holds the below functionality,

The  `offsetX` variable calculates the horizontal offset by dividing the width of the loveHeart div by 2. Similarly, the `offsetY` variable calculates the vertical offset by subtracting 55 pixels from half the height of the loveHeart div. Additionally, a `setTimeout` function is used to delay the execution of the `startHeartAnimation()` function by 5 seconds after the page loads.

> This animation is taken from this [Github repo](https://github.com/bennyxguo/h5-love). Credits to the
original creator. I tried out implementing unicolor functionality for the heart bloom, but doesn't actually work well. If you guys could implement that, fork my repo and submit a pull request.

### Glitter / Sparkle Cursor Animation

To implement the Sparkle Cursor animation, we could modify the HTML to:

```HTML

<script glitter-cursor="true" glitter-color="black" src="./dist/in-love.js"></script>

```

The `glitter-cursor` attribute is set to "true," enabling the glitter effect to interact with the cursor.

The `glitter-color` attribute is configured to specify the color of the glittering stars, with black chosen as the color in this example.

> Derived from this [Github repo](https://gist.github.com/averykhoo/8057a0324be445bd7eea32c89379eb76).
I modified the code to support glitter control, color input,  and made some changes in formatting.

<br>

# Contact

For any inquiries or further information, you can reach out to me through:

**Email**: [abineshmathivanan31@gmail.com](mailto:abineshmathivanan31@gmail.com)

**LinkedIn**: [Abinesh Mathivanan](https://www.linkedin.com/in/abineshmathivanan/)

**GitHub**: [Beens Github](https://github.com/Abinesh-Mathivanan)

<br>

# License

MIT License

Copyright (c) 2024 Beens

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

