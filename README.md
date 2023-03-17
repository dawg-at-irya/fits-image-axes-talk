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
In either case, I will show how this can be easily achieved either in pure matplotlib 
or by using libraries from Astropy. 

## Resumen
Cómo mostrar una imagen con ejes científicamente significativos en Python

Cuando usamos la función `imshow()` en Python matplotlib para mostrar una imagen, 
los ejes se muestran en unidades de píxeles por defecto.
Sin embargo, a menudo queremos mostrar la imagen usando otras unidades, 
como la longitud en parsecs o en coordenadas celestes.
En general, estas otras unidades se denominan _world coordinates_ (coordenadas mundiales).
A veces, la transformación de píxeles a coordenadas mundiales se proporciona en la cabecera de un archivo FITS,
pero ese no es siempre el caso.
En cualquier caso, mostraré cómo se puede lograr esto fácilmente en matplotlib puro o usando bibliotecas de Astropy.
