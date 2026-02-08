
# Textillate 2.0

A modern rewrite of Textillate.js powered by Anime.js.

**Created by Jacopo Mazzoni (2025)**  
Dedicated to the public domain under CC0 1.0.

# Usage
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/3.2.2/anime.min.js"></script>
    <script src="https://cdn.jsdelivr.net/gh/jacopomazzoni/textAnimate@master/src/TextillateAnime.js"></script> 
    <link rel="stylesheet" href="textillate-anime.css" />
  </head>
  <body>
    <div id="container">
      <h1 id="title">"There's no such thing as bad pizza</h1>
      <h1 id="subtitle">just pizza🍕"</h1>
    </div>
    <script>
      window.onload = () => {
        textillate("#title", {
          split: "chars",
          in: {
            effect: "flip",
            delayScale: 1.5,
            delay: 50,
            shuffle: false,
            sync: false,
          },
          out: { effect: "rotateOut", delay: 50, reverse: true },
          loop: true,
          minDisplayTime: 1200,
        });

        textillate("#subtitle", {
          split: "chars",
          in: {
            effect: "flip",
            delayScale: 1.5,
            delay: 150,
            shuffle: false,
            sync: false,
          },
          out: { effect: "rotateOut", delay: 50, reverse: true },
          loop: true,
          minDisplayTime: 1200,
        });
      };
    </script>
   </body>
  </html>
```

## License
CC0 1.0 Universal (Public Domain)

Inspired by the original Textillate.js by Jonathan Schroeder.
 
