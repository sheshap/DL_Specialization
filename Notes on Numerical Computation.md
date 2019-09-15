**Two types of Numerical errors**
1) Underflow - occurs when numbers close to zero are rounded off as zero.
2) Overflow - occurs when numbers with large magnitude are approximated as -&infin; or &infin;.

**Poor Conditioning**
Condition Number - ratio of the magintude of the largest and smallest eigenvalue.

**Gradient-Based Optimization**

**Objective function or criterion**
1) minimize f(x) --> cost/loss/error function.
2) gradient descent: reduce f(x) by moving x in small steps with the opposite sign of the derivative.
3) critical points/stationary points: provide no information about direction of gradient (f'(x) = 0).
4) local minimum: f(x) lower than all neighboring points, no longer possible to decrease f(x) by taking infinitesimal steps.
5) local maximum: f(x) higher than all neighboring points, no longer possible to increase f(x) by taking infinitesimal steps.
6) saddle points: critical points which are neither minima or maxima.
7) global minimum: absolute lowest value of f(x).
--------------------------------------------------------
8) gradient descent: positive gradient points uphill, negative gradient points downhill and f can be decreased by moving in the direction of negative gradient.
<p align="center">
x' = x - &epsilon;D<sub>x</sub>f(x)
</p>

9) Jacobian: matrix containing all partial first order derivatives of f.
10) Hessian: matrix containing all partial second order derivatives of f or partial first order derivatives of gradients.

Note: if second order derivative is
a) = 0 : no curvature, gradient 1, step size &epsilon; along the negative gradient, cost function decrease by &epsilon;.
b) < 0 : function curve downward, cost function decrease by more than &epsilon;.
c) > 0 : function curve upward, cost function decrease by less than &epsilon;.
