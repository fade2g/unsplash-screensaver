Simple web page that makes a "full browser window" unsplash screensaver

* On page load, it displays an image from [source.unsplash.com](https://source.unsplash.com)
* The image is filtered to be somewhat darker blue-grayish (currently, no need to have a dynamic filter)
* it does not reload an image after x seconds. Page refresh is the trigger
* By default, it takes images from the collection 2392731
* Through URL query parameters, the behaviour can be changed:
   * resize=*x*: when page loads, the image is resized from a bit bigger to fullscreen. *x* is the number of seconds for that animation (e.g. 5)
   * fadein=*y*: when page loads, the image color / brighness fades in from dark to, hmm, less dark. *y* is the numer of seconds for that animation (e.g. 5)
   * collection=*zzzzz*: Number of the unsplash colleciton, from which a random image is used
* query-parameters can be combined as needed
* E.g. `..../?resize=3&collection=12345` or `..../?resize=5&fadein=5`