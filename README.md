Build/Production code is located in the 'build' folder

Development code is in the 'development' folder


Summary of changes to index.html:

1) Removed Google Fonts
2) Made analytics.js and perfmatters.js async
3) Add media query to print stylesheet
4) Resized and optimized images with external tools
5) Inlined all css (with gulp-inline-css)

Summary of change to main.js for pizza.html:

1) Reduce # of pizzas to 30
2) moved " var phase = (document.body.scrollTop / 1250); " out of the for loop in the updatePositions() function
3) Resized and optimized images with external tools