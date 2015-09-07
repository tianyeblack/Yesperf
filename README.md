## Website Performance Optimization portfolio project

Usage: Click on index.html or visit my github page <http://tianyeblack.github.io/Yesperf>
###Part 1: Optimize PageSpeed Insights score for index.html

1. Minifying CSS and JS files, provided by PageSpeed;
1. Using JS to load small CSS file instead of blocking critical rendering process;
1. Making all the GA JS asynchronous because they need not to be executed right away or waiting for certain resources;
1. Minimizing the images used because there is no chance it will be that large on the front page;
1. Moving non-critical JS files to the end;
1. Giving "pring.css" a media tag;
1. Removing third-party font because they block the pipeline and are not worth the cost;

###Part 2: Optimize Frames per Second in pizza.html

1. Promoted the sliding pizzas to different layers so only they are repainted each time, trade painting off with layouts;
1. Reduced the sliding pizzas number to a reasonable one (depending on how large the window is);
1. Stored the values inside an array so there are way fewer forced layout invalidation;
1. Switch to getElementById and getElementsByClassName instead of queryBySelector;
1. Calculating the phase information first for there are always only 5 phases at a certain scroll position;
