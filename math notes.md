
## polynomials
- many names, non-negative and integer exponents needed in each use of variable
- 10x^7 - 9x^2 + 15x^3 + 9 --> 4 termed polynomial, coefficient of 10x^7 is 10
1. avg rate of change of f(x) = x^3 - 4x of range [-2,3] output [0,15] change between -2 and 3 is 5 so 15/5 = 3
- arc formula 
    - a =< x >= b
    - f(b) - f(a)/b - a

2. adding/subtracting polynomials
- like terms - terms with same variable to the same power, i.e. 5x^2 + 7x^2

- addition examples
(-4b^3 + b - 1) + (6b-6) = -4b^3 + 7b - 7
(-m^2 + 6) + (-4m^2 + 7m + 2) = -5m^2 + 7m + 8
(−5k^3 − 6k+1) + (−6k^2 + 5k) = -5k^3 - 6k^2 - k + 1
(−5x^2 + 6x + 7) + (−x^2 + 4x) = -6x^2 + 10x + 7

- subtraction examples
(3x^3 + 4x^2) − (2x^3 + 3x^2 − x) = (3x^3 + 4x^2) − 2x^3 - 3x^2 + x = x^3 + x^2 + x
(6a^3 + 7a^2) − (5a^3 + 9a^2 + a) = (6a^3 + 7a^2) − 5a^3 - 9a^2 - a = a^3 - 2a^2 - a  
(2k^3 + 6k + 1) − (2k^2 + 1) = (2k^3 + 6k + 1) − 2k^2 - 1 = 2k^3 - 2k^2 + 6k 
(2k^3 − 7k^2 + 3k) − (−4k^2 + 5k) = (2k^3 − 7k^2 + 3k) + 4k^2 - 5k = 2k^3 - 3k^2 - 2k

- more examples
(5a^2 − 6a − 4) - (-7a^2 + 3a - 9) = (5a^2 − 6a − 4) + 7a^2 - 3a + 9 = 12a^2 - 9a + 5 
(-7y^2 + 3y - 6) - (3y^2 + 4y + 4) = 

## tools
``` python

def arc(function, a, b):
    return ((function(b) - function(a))/(b-a))

```

``` python

```

#### worksheet
1. 
``` python
def f(x):
    return (x**3)-(4*x)

 x = -2
 y = 3   
```

``` python
def g(t):
    return -(t-1)**2 + 5  
```

``` python
def goo(x):
    return -((x**2)/4)+7  
```

``` python
def foo(x):
    return x**2 - x - 1
```

``` python
def fun(x):
    return (x**3) - (9*x)
```

``` python
def poly(x):
    return -((x**2)/4) + 7
```

``` python
def h(x):
    return (1/8)*(x**3) - x**2
```


``` python
def fun1(x):
    return -7*(x**2) + 3*x - 9

def fun2(x):
    return 5*(x**2) - 6*x -4
```