Website Performance Optimization Project
About

The objective for this project was to optimize Cameron Pittman's portfolio page for speed. The strategy was to optimize the critical rendering path, making the page render as quickly as possible, using techniques you've picked up in the Website Performance Optimization.

How to run

A live version of the site can be seen at www.free4thefree.net/udacity/frontend-nanodegree-mobile-portfolio.

Page load speed optimization

Image compression: images were rescaled and resized to better fit layout dimensions and thumbnails created where needed.
Inline critical CSS: critical above-the-fold content styles were inlined in the document vs. blocking loading. This was done using the methods prescribed by Google Developers (see references).
Defer alternative media CSS: print stylesheets were deliberately chosen not to be served inline in HTML documents due to at least three different pages using it. A media attribute was added to ensure that it would only be downloaded when printing.
Minify CSS/JS: all CSS and JS files were minified to ensure faster loading. The formatted files are still present in their respective directories, without the .min in their filenames.

Frame rate optimization

In views/js/main.js, unnecessary javascript operations were pulled out of for loops where possible.