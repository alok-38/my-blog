---
title: My Second Blog Post
author: Alokananda Y
description: "After learning some frontend development and Astro, I couldn't stop!"
image:
  url: "https://docs.astro.build/assets/arc.webp"
  alt: "The Astro logo on a dark background with a purple gradient arc."
pubDate: 2024-10-19
tags: ["astro", "blogging", "learning in public", "successes"]
---

# Let's Make a Cake: A Fun Web Project

In the world of web development, creating engaging and visually appealing content is key. Today, we’ll dive into a delightful project that combines HTML, CSS, and a sprinkle of creativity to create a cake-making page. This project is a part of the <a href="https://v2.scrimba.com/the-frontend-developer-career-path-c0j" target="_blank">Scrimba frontend career path.</a>

## Overview of the Project

The goal of this project is to build a simple, interactive web page that outlines the steps to make a cake. The page features fun graphics, clear instructions, and an animation that brings the content to life. Let’s break down the components of our project.

### HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cake Class</title>
    <link rel="stylesheet" href="style.css" />
    <script src="script.js" defer></script>
</head>
<body>
    <section>
        <h1>Let's make a Cake!</h1>
        <p>It's going to be a piece of cake</p>
        <ul class="grid">
            <li>🍓</li>
            <li>🍔</li>
            <li>🥛</li>
            <li class="scared">🥚</li>
            <li>🍣</li>
            <li>🍗</li>
            <li>🧈</li>
            <li>🥣</li>
        </ul>
        <h3>Directions</h3>
        <ol>
            <li>Preheat oven to 350 degrees F (175 degrees C).</li>
            <li>In a medium bowl, combine all ingredients.</li>
            <li>Pour batter into baking pan.</li>
            <li>Bake for 30 to 40 minutes in the preheated oven.</li>
            <li>Enjoy!</li>
        </ol>
    </section>
</body>
</html>
```

### Styling with CSS

```css
@import url("https://fonts.googleapis.com/css?family=Bubblegum+Sans&display=swap");

:root {
  --bg-color: #ecf2ff;
  --text-color: #2b283a;
  --title-color: #4a4e74;
}

body {
  background-color: var(--bg-color);
  font-family: sans-serif;
  color: var(--text-color);
  overflow: hidden;
}

section {
  width: 90%;
  margin: 0 auto;
}

h1 {
  color: var(--title-color);
  font-size: 3em;
  font-family: "Bubblegum Sans";
  text-align: center;
}

.grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: 70px;
}

.grid li {
  list-style-type: none;
  font-size: 3em;
  justify-self: center;
}

p {
  animation: moveAcross 15s linear infinite;
  position: relative;
}

@keyframes moveAcross {
  0% {
    left: -10%;
  }
  100% {
    left: 100%;
  }
}
```

<video width="640" height="360" controls>
  <source src="/public/cake_website.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

