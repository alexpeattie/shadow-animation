# Shadow animation jQuery plugin

## Easily animate box shadows

With this jQuery plugin, you can extend the animate function to support the CSS box shadow-property. You can animate the color, the x- and y-offset, the blur-radius and spread-radius. Mark Carver contributed code to support rgba-colors (the alpha channel).

## Example

Change the shadow to a centered 30-pixel blur with the color blue (#44f):

    $('#box1').animate({boxShadow: '0 0 30px #44f'});
    
## Restrictions

The plugin works in the current versions for Firefox, Safari and Chrome. It also works in the platform preview release of Internet Explorer 9.

Due to a [bug in Opera](http://www.bitstorm.org/jquery/shadow-animation/bugtest.html), it doesn't work in this browser. A bug report has been filed.

Currently, the shadow offset, blur and spread should be defined in pixels, so no ems, percentages etcetera. The plugin supports only one shadow.

## Release history

Version 1.5, released January 20th, 2011. Renamed shadow to boxShadow.

Version 1.4, released January 9th, 2011. Fixed support for elements without shadow set.

Version 1.3, released December 30th, 2010. Fixed support for alpha channel and negative offset.

Version 1.2, released October 3th, 2010. Fixed support for placing script in head.

Version 1.1, not released.

Version 1.0, released June 9th, 2010. First release.

## License

This jQuery-plugin is available under the [MIT and GPL License](http://www.bitstorm.org/jquery/license.html).