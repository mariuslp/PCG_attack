# PCG_attack
(Non optimal) Implementation in Sage of lattice reduction attacks on LCG and PCG


This is a proof of concept of Frieze, Hastad, Kannan et al.'s paper ([Reconstructing truncated integer variables satisfying linear congruences](https://www.math.cmu.edu/~af1p/Texfiles/RECONTRUNC.pdf)).
It can be used on a multiplicative LCG, or a general LCG. Exemples are given at the end of the source code.

Moreover, I added support for an attack on PCG ([PCG: A Family of Simple Fast Space-Efficient Statistically Good Algorithms for Random Number Generation](http://www.pcg-random.org/pdf/toms-oneill-pcg-family-v1.02.pdf)).
Even though resolution is quite slow on this generator (and my code could be greatly optimized), the computational security does not exceed 2^62 bits, way under the recommandations of the NIST (112 bits).
