# jGage
Rotating simple gages and dials with HMTL5 and jQuery UI

Starting with an image of a gage (in this case the ammeter for measuring amps on an electrical panel) position a canvas over top of it during the initialization property, see the set up function, eg position a 2d context, and rotate it as desired.

For the knob to be turned, load the image onto a canvas.  Using the jQuery slider called "range-min", make it invisible position it over the image.  Look for the element "#slider-range-min" to have a css style  " opacity:0 " and "z-index:3" to make this happen.  

The jQuery will add the event listeners for you and pass the values to any handlers you have specified.  Just add some functions see "dialer(val)" and "turndial(val) " that handle the turning and cal them from inside the slider object.  jQuery is nice for this since it adds the event listeners.  The slider gives it a nice feel for turning this kind of knob.
