**frontend-nanodegree-mobile-portfolio-project4**
**Frontend Project 4**
=======
## Website Performance Optimization portfolio project

**index.html** is the start page. From index.html you can view the other informatino Cameron mentioned like 2048 
PageSpeed Insights for **index.html**  http://chaz0468.github.io/project4.github.io
<ul>
	<li>Mobile: 95/100</li>
	<li>Desktop: 96/100</li>
</ul>
To achieve these scores I 
<ol>
<li>Resized the image pizzaria.jpg from its original size of 2048 x 1536 to 100 x 75 px</li>
    <li>changed data to my informatino vs camron)</li>
    <li>Minified print.css (print_mini.css)</li>
    <li>Added media="print" to print_mini.css ref</li>
    <li>In-lined my css file</li>
    <li>Added async to script references</li>
    <li>remmed out <link href="http://fonts.googleapis.com/css?family=Open+Sans:400,700" rel="stylesheet"></li>
 </ol>
 
 **pizza.html** achieve an FPS of 60 consistently when scrolling
 To achieve this I 
 <ol>
 	<li>Compressed the impages for the page the size of _pizza.png</li>
 	<li>Reduced the number of pizzas created from the original 200 down to 48</li>
 	<li> moved var's outside of loop for: function changePizzaSizes(size)</li>
 	<li>function updatePositions took the var's outside the forloop and cached varible to store method</li>
 	<li>In the _i_ var I assigned the beginning count to the length of the 'mover' items then decremented instead incremented </li>
 	<li>replaced querySelectorAll with getElementsByClassName in multiple spots</li>
 	
 </ol>
 
 **pizza.html** achieve 5ms or less when changing pizza sizes on slider. 
 <ol>
 	<li>Moved _var dx_ outside the _for_ loop of _changePizzaSizes_ function</li>
 	<li>Moved _var newidth_ outside the _for_ loop of _changePizzaSizes_ function</li>
 	<li>Moved _document.querySelectorAll(".randomPizzaContainer")_ outside the _for_ loop and assigned it to a newly created variable array called _elements_</li>
 	<li>For _var i_ I assigned a beginning value of the _elements_ (randomPizzaContainer) variable instead of zero, as we will always have at least one. I then decremented</li>
 </ol>
 
 **Resources**
 <ul>
 	<li><a href="https://developer.chrome.com/devtools/docs/demos/too-much-layout/index">Google Timeline demo</a></li>
 	<li><a href="https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fchaz0468.github.io%2Fproject4.github.io&tab=mobile">PageSpeed Insights</a></li>
 	<li><a href="https://developer.chrome.com/devtools/docs/network">Evaluating network performance</a></li>
 	<li><a href="http//jpeg-optimizer.com/">jpeg compressor</a></li>
 	<li><a href="http://tinypng.com">png compressor</a></li>
 	<li><a href="http://cssminify.com/">css minifier</a></li>
 </ul>

