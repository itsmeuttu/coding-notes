# Common Mathematical Symbols and Functions

### Algebraic Expressions

1. **Power and Square:**
    
    ```python
    x**2  # x squared
    x**3  # x cubed
    
    ```
    
2. **Square Root:**
    
    ```python
    sp.sqrt(x)  # square root of x
    
    ```
    
3. **nth Root:**
    
    ```python
    x**(1/3)  # cube root of x
    sp.root(x, 3)  # another way to get the cube root of x
    
    ```
    

### Exponential and Logarithmic Functions

1. **Exponential:**
    
    ```python
    sp.exp(x)  # e^x (exponential function)
    
    ```
    
2. **Natural Logarithm:**
    
    ```python
    sp.log(x)  # natural logarithm of x (ln(x))
    
    ```
    
3. **Logarithm with Base 10:**
    
    ```python
    sp.log(x, 10)  # logarithm of x with base 10
    
    ```
    
4. **Logarithm with Arbitrary Base:**
    
    ```python
    sp.log(x, 2)  # logarithm of x with base 2
    
    ```
    

### Trigonometric Functions

1. **Sine:**
    
    ```python
    sp.sin(x)  # sine of x
    
    ```
    
2. **Cosine:**
    
    ```python
    sp.cos(x)  # cosine of x
    
    ```
    
3. **Tangent:**
    
    ```python
    sp.tan(x)  # tangent of x
    
    ```
    
4. **Cotangent:**
    
    ```python
    sp.cot(x)  # cotangent of x
    
    ```
    
5. **Secant:**
    
    ```python
    sp.sec(x)  # secant of x
    
    ```
    
6. **Cosecant:**
    
    ```python
    sp.csc(x)  # cosecant of x
    
    ```
    

### Inverse Trigonometric Functions

1. **Inverse Sine (Arcsine):**
    
    ```python
    sp.asin(x)  # arcsine of x
    
    ```
    
2. **Inverse Cosine (Arccosine):**
    
    ```python
    sp.acos(x)  # arccosine of x
    
    ```
    
3. **Inverse Tangent (Arctangent):**
    
    ```python
    sp.atan(x)  # arctangent of x
    
    ```
    

### Hyperbolic Functions

1. **Hyperbolic Sine:**
    
    ```python
    sp.sinh(x)  # hyperbolic sine of x
    
    ```
    
2. **Hyperbolic Cosine:**
    
    ```python
    sp.cosh(x)  # hyperbolic cosine of x
    
    ```
    
3. **Hyperbolic Tangent:**
    
    ```python
    sp.tanh(x)  # hyperbolic tangent of x
    
    ```
    
4. **Hyperbolic Cotangent:**
    
    ```python
    sp.coth(x)  # hyperbolic cotangent of x
    
    ```
    
5. **Hyperbolic Secant:**
    
    ```python
    sp.sech(x)  # hyperbolic secant of x
    
    ```
    
6. **Hyperbolic Cosecant:**
    
    ```python
    sp.csch(x)  # hyperbolic cosecant of x
    
    ```
    

### Inverse Hyperbolic Functions

1. **Inverse Hyperbolic Sine:**
    
    ```python
    sp.asinh(x)  # inverse hyperbolic sine of x
    
    ```
    
2. **Inverse Hyperbolic Cosine:**
    
    ```python
    sp.acosh(x)  # inverse hyperbolic cosine of x
    
    ```
    
3. **Inverse Hyperbolic Tangent:**
    
    ```python
    sp.atanh(x)  # inverse hyperbolic tangent of x
    
    ```
    

### Other Useful Functions

1. **Absolute Value:**
    
    ```python
    sp.Abs(x)  # absolute value of x
    
    ```
    
2. **Sign Function:**
    
    ```python
    sp.sign(x)  # sign of x (returns -1, 0, or 1)
    
    ```
    
3. **Factorial:**
    
    ```python
    sp.factorial(x)  # factorial of x
    
    ```
    
4. **Gamma Function:**
    
    ```python
    sp.gamma(x)  # gamma function of x
    
    ```
    
5. **Beta Function:**
    
    ```python
    sp.beta(x, y)  # beta function of x and y
    
    ```
    
6. **Binomial Coefficient:**
    
    ```python
    sp.binomial(n, k)  # binomial coefficient (n choose k)
    
    ```
    

### Example Code Using Various Symbols and Functions

```python
import sympy as sp

# Define symbols
x, y, n, k = sp.symbols('x y n k')

# Expressions using various functions
square = x**2
square_root = sp.sqrt(x)
log_natural = sp.log(x)
log_base_10 = sp.log(x, 10)
sine = sp.sin(x)
cosine = sp.cos(x)
exponential = sp.exp(x)
absolute_value = sp.Abs(x)
factorial_expr = sp.factorial(n)
binomial_coeff = sp.binomial(n, k)

# Display the expressions
print(f"x squared: {square}")
print(f"Square root of x: {square_root}")
print(f"Natural logarithm of x: {log_natural}")
print(f"Logarithm of x with base 10: {log_base_10}")
print(f"Sine of x: {sine}")
print(f"Cosine of x: {cosine}")
print(f"Exponential of x: {exponential}")
print(f"Absolute value of x: {absolute_value}")
print(f"Factorial of n: {factorial_expr}")
print(f"Binomial coefficient (n choose k): {binomial_coeff}")

```

### Output:

```
x squared: x**2
Square root of x: sqrt(x)
Natural logarithm of x: log(x)
Logarithm of x with base 10: log(x, 10)
Sine of x: sin(x)
Cosine of x: cos(x)
Exponential of x: exp(x)
Absolute value of x: Abs(x)
Factorial of n: factorial(n)
Binomial coefficient (n choose k): binomial(n, k)

```

This guide provides a comprehensive overview of how to write various mathematical expressions using SymPy, covering a wide range of functions and operations.