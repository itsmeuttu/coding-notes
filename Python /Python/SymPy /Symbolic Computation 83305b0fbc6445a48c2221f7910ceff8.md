# Symbolic Computation

### Common SymPy Expressions and Functions

1. **Installing SymPy:**
    
    ```bash
    pip install sympy
    
    ```
    
2. **Importing SymPy:**
    
    ```python
    import sympy as sp
    
    ```
    
3. **Defining Symbols:**
    
    ```python
    x, y, z = sp.symbols('x y z')
    
    ```
    
4. **Defining Functions:**
    
    ```python
    f = x**2 + y**2
    g = sp.sin(x) * sp.exp(y)
    
    ```
    
5. **Algebraic Manipulations:**
    - **Expand:**
        
        ```python
        expanded = sp.expand((x + y)**3)
        print(f"Expanded: {expanded}")
        
        ```
        
    - **Factor:**
        
        ```python
        factored = sp.factor(x**3 - x**2 + x - 1)
        print(f"Factored: {factored}")
        
        ```
        
    - **Simplify:**
        
        ```python
        simplified = sp.simplify((x**2 - y**2) / (x - y))
        print(f"Simplified: {simplified}")
        
        ```
        
6. **Calculus Operations:**
    - **Derivative:**
        
        ```python
        derivative = sp.diff(f, x)
        print(f"Derivative of {f} with respect to x: {derivative}")
        
        ```
        
    - **Integral:**
        
        ```python
        integral = sp.integrate(f, x)
        print(f"Integral of {f} with respect to x: {integral}")
        
        ```
        
    - **Definite Integral:**
        
        ```python
        definite_integral = sp.integrate(f, (x, 0, 1))
        print(f"Definite integral of {f} from 0 to 1: {definite_integral}")
        
        ```
        
    - **Limit:**
        
        ```python
        limit = sp.limit(sp.sin(x) / x, x, 0)
        print(f"Limit of sin(x)/x as x approaches 0: {limit}")
        
        ```
        
7. **Solving Equations:**
    
    ```python
    equation = sp.Eq(x**2 + y, 1)
    solutions = sp.solve(equation, x)
    print(f"Solutions to the equation {equation}: {solutions}")
    
    ```
    
8. **Matrix Operations:**
    
    ```python
    matrix = sp.Matrix([[1, 2], [3, 4]])
    determinant = matrix.det()
    inverse = matrix.inv()
    print(f"Matrix: {matrix}")
    print(f"Determinant: {determinant}")
    print(f"Inverse: {inverse}")
    
    ```
    
9. **Series Expansion:**
    
    ```python
    series = sp.series(sp.sin(x), x, 0, 10)
    print(f"Series expansion of sin(x) around x=0: {series}")
    
    ```
    
10. **Substitution:**
    
    ```python
    substituted = f.subs(x, 1)
    print(f"Substituting x=1 in {f}: {substituted}")
    
    ```
    

### Example: Integrating and Simplifying an Expression

Combining some of the above operations into a coherent example:

```python
import sympy as sp

# Define the variable
x = sp.symbols('x')

# Define the function to integrate
f = x**2

# Perform the indefinite integration
integral = sp.integrate(f, x)

# Simplify the integral
integral_simplified = sp.simplify(integral)

# Display the result
print(f"The integral of {f} with respect to x is {integral_simplified}")

# Perform the definite integration from 0 to 1
definite_integral = sp.integrate(f, (x, 0, 1))

# Display the definite integral result
print(f"The definite integral of {f} from 0 to 1 is {definite_integral}")

# Evaluate the definite integral numerically
definite_integral_evaluated = definite_integral.evalf()

# Display the numerical evaluation
print(f"The numerical evaluation of the definite integral is {definite_integral_evaluated}")

```

### Output:

```
The integral of x**2 with respect to x is x**3/3
The definite integral of x**2 from 0 to 1 is 1/3
The numerical evaluation of the definite integral is 0.333333333333333

```