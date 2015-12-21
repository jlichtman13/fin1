#Precision loss

Equation (5) loses it precision due to the usage of a term that approaches zero.  In the numerator there is a sqrt(1-sin^2 a) term
which is the cause for the loss in precision.  This is becuase, as is well know, that sin cannot exceed a value of 1. Yet, despite
this it can still get very close to 1,-1, and 0, making it apparant that the term will approach zero at some points, 1 at some points
and 2 at some points.  When the term approaches one it creates the situation in which the entire numerator is effectively zero, which
when dealing with a computer language will cause an extreme loss of precision like that which is seen.
