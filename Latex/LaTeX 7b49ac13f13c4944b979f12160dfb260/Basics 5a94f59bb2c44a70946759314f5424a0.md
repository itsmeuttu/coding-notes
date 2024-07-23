# Basics

LaTeX is a typesetting system that is widely used for creating scientific and technical documents, such as research papers, articles, books, and presentations. It is known for its high-quality output, flexibility, and powerful features for creating complex mathematical equations, tables, and figures.

### 1. Creating a basic document:

- A LaTeX document begins with a preamble that specifies the document class, packages, and settings.
- The \documentclass{} command specifies the type of document, such as article, book, or report.
- The \usepackage{} command loads additional packages that provide extra functionality, such as graphics, fonts, and special symbols.
- The main content of the document is enclosed in the \begin{document} and \end{document} commands.

### 2. Formatting text:

- LaTeX provides commands for formatting text, such as
- \textbf{} for bold
    
    ```latex
    eg: \textbf{Happy}
    ```
    
    $$
     \textbf{Happy}
    $$
    
- \emph{} for italic
    
    ```latex
                                  eg: \emph{Happy}
    ```
    
- \underline{} for underline

```latex
eg: \underline{Hapapy}
```

 

$$
\underline{Hapapy}
$$

- LaTeX also allows you to control the font size and typeface using commands like \fontsize{} and \fontfamily{}.

### 3. Creating lists:

- LaTeX provides several types of lists, such as itemized, enumerated, and description lists.
- Lists are created using the \begin{itemize}, \begin{enumerate}, and \begin{description} commands, respectively.

### 4. Creating equations:

- LaTeX provides a powerful syntax for creating mathematical equations, using commands like \frac{}, \sqrt{}, and \sum{} and many more.
- Equations can be numbered using the \begin{equation} and \end{equation} commands, or unnumbered using the \begin{equation*} and \end{equation*} commands.
    
    Here are some examples of LaTeX code for math:
    
    1. Fractions:
    
    ```latex
    
    $\frac{numerator}{denominator}$
    
    Example: $\frac{3}{4}$
    ```
    
    $$
    \frac{a}{b}
    $$
    
    1. Exponents:
    
    ```latex
    
    $a^{exponent}$
    
    Example: $2^{10}$
    ```
    
    $$
    2^{10}
    $$
    
    1. Subscripts:
    
    ```latex
    
    $a_{subscript}$
    
    Example: $x_{n+1}$
    ```
    
    $$
    a_{n+1}
    $$
    
    1. Roots:
    
    ```latex
    
    $\sqrt{expression}$
    
    Example: $\sqrt[3]{2}$
    ```
    
    $$
    \sqrt[3]{2}
    $$
    
    1. Integrals:
    
    ```latex
    
    $\int_{lower}^{upper} expression dx$
    
    Example: $\int_{0}^{\infty} e^{-x} dx$
    
    ```
    
    $$
    \int_{0}^{\infty} e^{-x} dx
    $$
    
    1. Summations:
    
    ```latex
    
    $\sum_{i=lower}^{upper} expression$
    
    Example: $\sum_{i=1}^{n} i^2$
    ```
    
    $$
    \sum_{i=1}^{n} i^2
    $$
    
    1. Matrices:
    
    ```latex
    
    \begin{matrix}
    a & b \\
    c & d
    \end{matrix}
    
    Example: \begin{matrix}
    3 & 4 \\
    5 & 6
    \end{matrix}
    ```
    
    $$
    \begin{matrix}
    3 & 4 \\
    5 & 6
    \end{matrix}
    $$
    
    1. Derivatives:
    
    ```latex
    
    $\frac{d}{dx} expression$
    
    Example: $\frac{d}{dx} x^2$
    
    ```
    
    $$
    Example: \frac{d}{dx} x^2
    $$
    
    1. Limits:
    
    ```latex
    
    $\lim_{x \to a} expression$
    
    Example: $\lim_{x \to 0} \frac{\sin x}{x}$
    
    ```
    
    $$
    \lim_{x \to 0} \frac{\sin x}{x}
    $$
    
    1. Piecewise functions:
    
    ```latex
    
    $f(x) =
    \begin{cases}
    1 & x \geq 0 \\
    0 & x < 0
    \end{cases}$
    
    ```
    
    $$
    f(x) =
    \begin{cases}
    1 & x \geq 0 \\
    0 & x < 0
    \end{cases}
    $$
    
    ### 4. Creating tables:
    
    - LaTeX provides a simple syntax for creating tables, using the \begin{tabular} and \end{tabular} commands.
    - Tables can be formatted using various options, such as vertical and horizontal lines, cell alignment, and column width.
        
        ```latex
        
          
            \begin{tabular}{|c|c|c|}
            \hline
            Column 1 & Column 2 & Column 3 \\
            \hline
            Item 1   & A        & 10 \\
            Item 2   & B        & 20 \\
            Item 3   & C        & 30 \\
            \hline
            \end{tabular}
         
        ```
        
        ### 5. Greek Letters
        
        Here are the Greek letters and their corresponding LaTeX notation:
        
        ```latex
        \documentclass{article}
        
         \begin{document}
         Alpha: $\alpha$\\
        Beta: $\beta$\\
        Gamma: $\gamma$\\
        Delta: $\delta$\\
        Epsilon: $\epsilon$\\
        Zeta: $\zeta$\\
        Eta: $\eta$\\
        Theta: $\theta$\\
        Iota: $\iota$\\
        Kappa: $\kappa$\\
        Lambda: $\lambda$\\
        Mu: $\mu$\\
        Nu: $\nu$\\
        Xi: $\xi$\\
        Omicron: $o$\\
        Pi: $\pi$\\
        Rho: $\rho$\\
        Sigma: $\sigma$\\
        Tau: $\tau$
        Upsilon: $\upsilon$\\
        Phi: $\phi$\\
        Chi: $\chi$\\
        Psi: $\psi$\\
        Omega: $\omega$\\
         \end{document}
        ```
        
        ```
        Alpha: α
        Beta: β
        Gamma: γ
        Delta: δ
        Epsilon: ε
        Zeta: ζ
        Eta: η
        Theta: θ
        Iota: ι
        Kappa: κ
        Lambda: λ
        Mu: μ
        Nu: ν
        Xi: ξ
        Omicron: o
        Pi: π
        Rho: ρ
        Sigma: σ
        Tau: τ Upsilon: υ
        Phi: φ
        Chi: χ
        Psi: ψ
        Omega: ω
        
        ```
        

### 6. Use of def syntax

If you have alot of same math lang then we use \def syntax for easiness.

| \def | $x^2 +x^2$ | \def\foo{x^2} \foo + \foo |
| --- | --- | --- |