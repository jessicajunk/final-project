final-project
=============
Ticket #11493. Fix the wrong integral computation.  The problem seems to be with the types, reals and rationals.

integrate(x^(0.5)*e^(-x-x^2),x,0,infinity).n()
-->  0.886226925452758

integrate(x^(1/2)*e^(-x-x^2),x,0,infinity).n()
-->  0.32015709036013135
