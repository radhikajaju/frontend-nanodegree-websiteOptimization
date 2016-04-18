## Website Performance Optimization portfolio project

###Objective:
To optimize online portfolio for speed! In particular, optimize the critical rendering path and make the page render as quickly as possible.

### Getting started
##SETUP before you start your project!

1. Fork the repository.
2. To inspect the site on your phone, you have to run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```
3. Open a browser and visit localhost:8080
4. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok http 8080
 
  ```
  ###After connection is established Tunnel will be active.

5. Copy the public URL or HTTPS URL ngrok gives you and try running it through PageSpeed Insights! 
Profile, optimize, measure... and then lather, rinse, and repeat. Good luck!


####Part 1: Optimized index.html score by using PageSpeed Insights.

1. Checked PageSpeed Insight for score on mobile and desktop devices.
2. Recorded the timeline to figure out jank.
3. Reduced image size of all the images by using ImageOptim application.
4. Inlined CSS in index.html
5. Added media="print" to avoid render blocking CSS.
6. Shifted all the JavaScript at the bottom for smooth rendering of page.
7. Added async to GoogleAnalytics script tag.

####Part 2: Optimize Frames per Second in views/pizza.html and modify until FPS becomes 60 or higher.

1. Recorded timeline.
2. Saw a red triangle on Layout indicated Forced Synchronoused Layout in Main.js
3. Made changes in UpdatePosition() and changePizza Sizes().
4. Added comments for easy understanding.
5. minified all the HTML ,CSS and JavaScript files.

### Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")