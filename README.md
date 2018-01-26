# Website Performance Optimization portfolio project
----------------------------
# About
The purpose of this project is to optimize this online portfolio for speed In particular, optimize the critical rendering path and make this page render in speed of at least 90 scores for both mobile and desktop view for `index.html` and run `pizza.html` at 60fps when scrolling.

---------------------------
# Getting started
In order for you to run this site :
- You can download all the files from [my repo](https://github.com/osamaalfaify/frontend-nanodegree-mobile-portfolio) and open `index.html` in your web browser.
- You can just [click here](https://osamaalfaify.github.io/frontend-nanodegree-mobile-portfolio/)
---------------------------
# Changes made to optimize this site :
# Part 1: Optimize PageSpeed Insights score for index.html
- Use `async` attribute to stop JS from blocking the rendering path by synchronously loading low priority scripts.
- Place the function inside `<script>` at the bottom of the `<body>`
- Remove the web font as it can slow the page down.
- Compress the images to reudce their size.
- Resize the pizza image.
- Use media querie `media="print"` for the external `print.css` sheet as you don't need it to load every time you open the page unless you are planning on printing.
---------------------------

# Part 2: Optimize Frames per Second in pizza.html
- Take almost the `var` declerations out of loops.
- Take some calculations out of loops as we don't need them to recalculate with every iteration when the result is always the same.
- compress all images.
- Minify JS and CSS files.
- Change every `querySelector` with `getElementById` cause it's faster.
- Save the array length in a varibale `Length`, so the value isn't checked with every iteration.
---------------------------
# Results

# Desktop `index.html` score :
93/100
- https://github.com/OsamaAlfaify/frontend-nanodegree-mobile-portfolio/blob/master/screenshots/Screen%20Shot%202018-01-27%20at%201.00.30%20AM.png

# Mobile `index.html` score :
99/100
- https://github.com/OsamaAlfaify/frontend-nanodegree-mobile-portfolio/blob/master/screenshots/Screen%20Shot%202018-01-27%20at%201.00.34%20AM.png

# Resources & Tools:
* [page speed insight](https://developers.google.com/speed/pagespeed/)
* [for image optimizing](http://optimizilla.com/)
* [JavaScript minifier](https://javascript-minifier.com/)
* [CSS minfier](https://cssminifier.com/)
* [JS beautifier](http://jsbeautifier.org/)
* [pic resize](http://picresize.com/)
* [GitHub pages](https://pages.github.com/)
