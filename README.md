## Website Performance Optimization portfolio project

####Part 1: Optimize PageSpeed Insights score for index.html

1. Reduce the size and of pizzeria.jpg and profilepic.jpg manually and then use the version provided by PageSpeed Insights
1. Inline style.css
1. Specify media for print.css
1. Add async for analytic.ss
1. Remove the link for google web fonts and add the font in the inline part of style.css
1. Minify js and css with yuicompressor
    java -jar ~/udacity/yuicompressor-2.4.8.jar -v -o '.css$:-min.css' *.css
    java -jar ~/udacity/yuicompressor-2.4.8.jar -v  -o '.js$:-min.js' *.js
1. Minify index.html

####Part 2: Optimize Frames per Second in pizza.html

1. Replace querySelector and querySelectorAll with getElementById and getElementsByClassName.  Also move these function calls out of the loop.
1. Reduce the number of pizzas in addEventListener from 200 to rows and columns based on screen size
1. Move the math function out of the loop.  Pre-calculate the 5 possible values in updatePositions
1. Use translateX to move pizzas instead of incrementing style.left.
1. Add translate3d layer
1. Move the calculation of newwidth out of the loop in changePizzaSizes()

