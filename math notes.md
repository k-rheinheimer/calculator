
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
(-7y^2 + 3y - 6) - (3y^2 + 4y + 4) = (-7y^2 + 3y - 6) - 3y^2 - 4y - 4 = -10y^2 -y - 10
(8x^2 − 6x + 2) - (3x^2 + 7x + 4) = (8x^2 − 6x + 2) - 3x^2 - 7x + 4 = 5x^2 - 13x + 6
(7x^2 - 3x + 10) - (-4x^2 + 6x - 4) = (7x^2 - 3x + 10) + 4x^2 - 6x + 4 = 11x^2 - 9x + 14


3. multiplication
**A. multiply monomials/monomials by polynomials**
- like terms get multiplied add exponents
(5x^2)(3x^5) = 15x^7
- find area monomial * polynomial, a = w*l
4x^3(x^3+3x^2+2x) = 4x^6 + 12x^5 + 8x^4

**B. mutiply binomials by polynomials**
- find area:
(-6y + y^2)(3y^2 - 2y + 1) = -18y^3 + 3y^4 + 12y^2 - 2y^3 - 6y + y^2 = 3y^4 - 20y^3 + 13y^2 - 6y
(x + 9)(x^2 + 2x) = x^3 + 9x^2 + 2x^2 + 18x = x^3 + 11x^2 + 18x
(b^3 + b^2)(b^2 + 7b + 4) = b^5 + b^4 + 7b^4 + 7b^3 + 4b^3 + 4b^2 = b^5 + 8b^4 + 11b^3 + 4b^2

- scratch for quiz
(w^2 + 2)(w^2 + 3w + 9)
w^4 + 2w^2 + 3w^3 + 6w + 9w^2 + 18 = w^4 + 3w^3 + 11w^2 + 6w + 18 

(r^2 - 7)(-r^2 + 3r - 7) = (-r^4 + 7r^2) + (3r^3 - 21r) - (7r^2 - 49) +

2w^2 + 12w + 18
3w^3 + 18w^2 + 27w


(8w^4 + w^3)(8w^4 + w^3) = 64w^8 + 8w^7 + 8w^7 + w^6 = 64w^8 + 16w^7 + w^6

(4d^2 - 2d^7)(4d^2 - 2d^7) = 16d^4 - 8d^9 - 8d^9 - 4d^14


## tools
``` python

def arc(function, a, b):
    return ((function(b) - function(a))/(b-a))

```


#### attempt at polynomial arithmetic function
``` python 
# from functools import reduce
# def composite_addition(*func):  
#     def compose(a, b):
#         return lambda x : a(b(list(x)))
#     return reduce(compose, func, lambda : x)

# def add(A, B, m, n):
#     size = max(m, n);
#     sum = [0 for i in range(size)]     
#     for i in range(0, m, 1):
#         sum[i] = A[i]
#     for i in range(n):
#         sum[i] += B[i]
#     return sum

# def source_poly(poly, n, var: str):
#     resultset = []
#     for i in range(n):
#         x = poly[i]
#         if (i != 0):
#             monomial = str(x) + str(str(var)+'^' + str(i)) + ' +' 
#             resultset.append(monomial)
#     resultset[-1] = resultset[-1].replace(' +','')    
#     return resultset


# def construct_poly_string(*args: list):
#     for arg in args:
#         return ' '.join(arg)        

# add_poly = composite_addition(construct_poly_string, source_poly, add)

# A = [5, 0, 10, 6]
# B = [1, 2, 4]
# m = len(A)
# n = len(B)   
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