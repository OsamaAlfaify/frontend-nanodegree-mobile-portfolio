## Website Performance Optimization portfolio project
----------------------------
## About
The purpose of this project is to optimize this online portfolio for speed In particular, optimize the critical rendering path and make this page render in speed of at least 90 scores for both mobile and desktop view for `index.html` and run `pizza.html` at 60fps when scrolling.

---------------------------
### Getting started
In order for you to run this site :
1- You can download all the files from [my repo](https://github.com/osamaalfaify/frontend-nanodegree-mobile-portfolio) and open `index.html` in your web browser.
2- You can just [click here](https://osamaalfaify.github.io/frontend-nanodegree-mobile-portfolio/)
---------------------------
### Changes made to optimize this site :
# Part 1: Optimize PageSpeed Insights score for index.html
1- Use `async` attribute to stop JS from blocking the rendering path by synchronously loading low priority scripts.
2- Place the function inside `<script>` at the bottom of the `<body>`
4- Remove the web font as it can slow the page down.
5- Compress the images to reudce their size.
6- Resize the pizza image.
7- Use media querie `media="print"` for the external `print.css` sheet as you don't need it to load every time you open the page unless you are planning on printing.
---------------------------

# Part 2: Optimize Frames per Second in pizza.html
1- Take almost the `var` declerations out of loops.
2- Take some calculations out of loops as we don't need them to recalculate with every iteration when the result is always the same.
3- compress all images.
4- Minify JS and CSS files.
5- Change every `querySelector` with `getElementById` cause it's faster.
6- Save the array length in a varibale `Length`, so the value isn't checked with every iteration.
---------------------------
### Results

##### Desktop `index.html` score :
93/100

##### Mobile `index.html` score :
99/100

### Resources & Tools:
* [page speed insight](https://developers.google.com/speed/pagespeed/)
* [for image optimizing](http://optimizilla.com/)
* [JavaScript minifier](https://javascript-minifier.com/)
* [CSS minfier](https://cssminifier.com/)
* [JS beautifier](http://jsbeautifier.org/)
* [pic resize](http://picresize.com/)
* [GitHub pages](https://pages.github.com/)
