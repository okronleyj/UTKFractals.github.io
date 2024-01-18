Link to website: https://okronleyj.github.io/UTKFractals.github.io/

#UTKFractals.github.io

This is the readme file for the website created my Jordan O'Kronley for the UTK YETI challenge in Jan 2024.

I've never made a website before so this was a fun project full of learning.  That being said, it's very poorly coded and not optimized at all.

The website is all about fractals and I use 3 examples of fractals to teach the users about them.  These 3 examples are the Mandelbrot set, the weierstrass function, and the coastal paradox.

### Mandelbrot set ###
Wiki: https://en.wikipedia.org/wiki/Mandelbrot_set

This is probably the most well known fractal.  It takes an iterative algorithm and deterimes when the algoirthm diverges.  The function is

f(z) = z^2+c

where c is a constant complex number.  The algorithm is

f_0(0) = 0 + c
f_1(f_0) = c^2 + c
f_2(f_1(f_0)) = (c^2+c)^2+c
...

The html code basically goes through every point on a canvas and performs this algorithm using each pixel as a new "c" value.  The user can then move the plot around and adjust the resolution which cause the webpage to recalculate the algorithm to display.

### Weierstrass function ###
Wiki: https://en.wikipedia.org/wiki/Weierstrass_function

This is an interesting function in mathmatics but not as flashy as the other 2 examples.  

THe weierstrass function is an infinite sum of cosines where the sum is continuous but not differentiable.  This section just plots the first "n" terms of this function and lets the user see that the function is continuous but the fractal nature of the function causes sharp, non-differentialbe points.

### Coastal paradox ###
Wiki: https://en.wikipedia.org/wiki/Coastline_paradox

This section was definitly the most painful to code.  I originally wanted to generate a random shape (colleciton of points) and then generate a coastline wraping up all the points.  Generating this coastline is known as a concave hull which is an extremely difficult task to do.  The only way to implement it would be by paying for already built software or spending months building my own code from multiple numerical papers.

I then found out about GeoJson files that contain the coastline data of real world countries.  This website has the GeoJson files I used for the US coastlines:

https://eric.clst.org/tech/usgeojson/

This website had multiple resolutions of the coastline which I could create buttons for and have the user switch between.  The user can see that by increasing the resolution, the coastline gets longer.








