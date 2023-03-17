# How to display an image with scientifically meaningful axes in Python

Short presentation to be given by Will Henney at DAWGI, Morelia meeting 2023-03-22

## Summary
When we use the Python matplotlib function `imshow()` to display an image,
the axes are shown in pixel units by default. 
However, we often want to display the image using some other units,
such as length in parsecs or in celestial coordinates. 
In general, these other units are called _world coordinates_.
Sometimes the transformation from pixels to world coordinates is given in the header of a FITS file,
but that is not always the case. 
In either case, 
I will show this can be easily achieved in either in pure matplotlib 
or using libraries from Astropy. 
