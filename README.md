## Website Performance Optimization portfolio project

### Getting started

Some useful tips to help you get started:
#### local server
1. Check out the repository
2. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m http.server 8080
  ```

3. Open a browser and visit localhost:8080

#### remote server
1. Download and install [ngrok](https://ngrok.com/) to the top-level of your project directory to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ./ngrok http 8080
  ```

### Part 1: Optimize PageSpeed Insights score for index.html

Optimization step:
1. inline css, media css as it neednot reload at the beginning
2. downloads online javascript, async javascript
3. async google fonts
4. compress the img of picture，compress css if needed
6. run pagespeed, optimize again


### Part 2: Optimize Frames per Second in pizza.html
optimize views/pizza.html, and views/js/main.js to match frames per second rate is 60 fps or higher.

Optimization step:
1. run google chrome performance, and get the fps, check the call function with bad performance
2. find detail lines in the call function with bad performance
3. modify the js code
4. run performance and optimize again
4. check other performance, when do more operation: reload page, reflash the page, enlarged and reduce the page and so on
5. check and modify the call function(main.js), such as for loop, comments and so on.
