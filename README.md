# Shadow animation jQuery plugin

## Easily animate box shadows

With this jQuery plugin, you can extend the animate function to support the CSS box shadow-property. You can animate the color, the x- and y-offset, the blur-radius and spread-radius. Mark Carver contributed code to support rgba-colors (the alpha channel). Alex Peattie contributed code to support other units (em and pt), and some misc. fixes.

## Example

Change the shadow to a centered 30-pixel blur with the color blue (#44f):

    $('#box1').animate({boxShadow: '0 0 30px #44f'});
    
## Restrictions

The plugin works in the current versions for Firefox, Safari and Chrome. It also works in the platform preview release of Internet Explorer 9.

Due to a [bug in Opera](http://www.bitstorm.org/jquery/shadow-animation/bugtest.html), it doesn't work in this browser. A bug report has been filed.

If setting the opacity of a shadow to 0, you should instead use a very small number like 0.01 (otherwise Firefox will lose the shadow's color information), like so:

    .animate({boxShadow: 0 0 10px rgba(255,0,255,0.01)});

Currently, the shadow offset, blur and spread should be defined in pixels, ems or pts. Percentages and [other units](https://developer.mozilla.org/en/CSS/length) are unsupported. The plugin currently supports only one shadow.

## Release history

Version 1.6, released March 11th, 2011. Added support for em and pt. Other minor fixes.

Version 1.5, released January 20th, 2011. Renamed shadow to boxShadow.

Version 1.4, released January 9th, 2011. Fixed support for elements without shadow set.

Version 1.3, released December 30th, 2010. Fixed support for alpha channel and negative offset.

Version 1.2, released October 3th, 2010. Fixed support for placing script in head.

Version 1.1, not released.

Version 1.0, released June 9th, 2010. First release.

## License

This jQuery-plugin is available under the [MIT and GPL License](http://www.bitstorm.org/jquery/license.html).