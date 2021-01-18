# MathFunctions
Replacements of C/C++ standard library math functions for consistency and performance

## Primary functions:
**`cos_quarters(double x)`**: Returns cosine of `x`, where `x` is an angle expressed in quarter turns, so `x`=4 would represent a full turn (360 degrees or tau radians).  This is exact for multiples of 1 quarter turn.

**`sin_quarters(double x)`**: Returns sine of `x`, where `x` is an angle expressed in quarter turns.  This is exact for multiples of 1 quarter turn.

**`cos_sin_quarters(double x, double* cos_sin)`**: Fills in the first `double` pointed to by `cos_sin` with the cosine of `x`, and the second with the sine of `x`, where `x` is an angle expressed in quarter turns.  This is exact for multiples of 1 quarter turn, i.e. integer `x`.

**`atan_eighths(double y)`**: Returns inverse tangent of `y`, in eighths of a turn, so slope `y`=1 would yield a result of 1 eighth of a turn (45 degrees or tau/8 radians).  This is exact for -1, 0, 1, and infinities, producing values -1, 0, 1, and -2 or 2, respectively.  Its output range is `[-2,2]`.

**`atan2_eighths(double y, double x)`**: Returns two-argument inverse tangent of `y/x`, in eighths of a turn, so `y`=-5 and `x`=-5 would yield a result of -3 eighths of a turn (-135 degrees or (-3/8)tau radians).  This is exact for integer output values.  Its output range is `[-4,4]`.

**`exp2(double x)`**: Returns 2 to the power of `x`.  This is exact for values of `x` that are integers.

**`cube_root(double x)`** Returns the cube root of `x`.  This is exact for values of `x` that are integer powers of 8, (including `x`=1, since that is 8 to the power of zero.)
