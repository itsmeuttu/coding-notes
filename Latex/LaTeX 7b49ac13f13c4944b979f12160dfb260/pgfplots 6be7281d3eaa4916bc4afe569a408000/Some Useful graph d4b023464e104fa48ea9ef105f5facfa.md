# Some Useful graph

# Sin x graph

```latex
\documentclass{article}
\usepackage{pgfplots}

\begin{document}

\begin{tikzpicture}
\begin{axis}[
    title={Graph of $\sin x$},
    axis lines=center,
    xlabel=\empty,
    ylabel={},
    ymax=1,
    ymin=-1,
    xmin=0,
    xmax=2*pi,
    ytick={-1, 0, 1}, 
    yticklabels={-1, 0, 1}, 
    domain=0:2*pi,
    samples=100,
    xtick={0, pi/2 , pi, 3*pi/2, 2*pi},
    xticklabels={$0$, $\frac{\pi}{2}$, $\pi$, $\frac{3\pi}{2}$, $2\pi$},
    legend pos = north east
]

\addplot[blue, smooth]{sin(deg(x))};
\legend{$\sin x$}

\end{axis}
\end{tikzpicture}
\end{document}
```

## Output

![Untitled](Some%20Useful%20graph%20d4b023464e104fa48ea9ef105f5facfa/Untitled.png)