#Energy compression comparision between different transforms by plotting them 

.......
problem statement 

.take a 64 length sequence do dft,dct,haar transform to it.

.make L high frequency components to zero

.vary L from 0 to length 

.for each L compute inverse transform after making L components from dft,dct,haar to zero

.compute mse between original sample and value from inverse

plot mse vs L 
.......

....
$$ implementation details
function dft,dct,haar,idft,idct,ihaar compute matrices for transforms

function generalised fourier transform and inverse generalised fourier transform computes dft,dct,haar transform and inverse dft,dct,haar on transformed sample

mse calculates error mean square error

dot_product simply computes dot product between 2 vectors and divide it by vector length

xdft,xdcthaar makes L components to zero
