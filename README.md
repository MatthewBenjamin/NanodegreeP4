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
4) Moved the following calculations out of for loops:
    a) var windowwidth = document.querySelector("#randomPizzas").offsetWidth (determineDX function)
    b) document.querySelectorAll(".randomPizzaContainer") (changePizzaSizes function)
    c) var dx = determineDx(document.querySelectorAll(".randomPizzaContainer")[i], size) (changePizzaSizes function)
    d) var newwidth = (document.querySelectorAll(".randomPizzaContainer")[i].offsetWidth + dx) + 'px' (changePizzaSizes function)

Summary of changes to views/css/style.css
1)   Added "max-width: 73.333px" & "max-height: 100px" to "mover" class, removed "width: 256px"