# Basic shape: Drawing a rectangle

```latex
\documentclass{article}
\usepackage{tikz}

\begin{document}
\begin{tikzpicture}
  \draw (0, 0) rectangle (4, 2);
\end{tikzpicture}
\end{document}
```

Output: 

![Untitled](Basic%20shape%20Drawing%20a%20rectangle%20f478ee3485094c1cbe5a8f0adf301ca6/Untitled.png)

## /draw

The **`\draw`** command is one of the core commands provided by the TikZ package in LaTeX. It is used for creating various graphical elements, such as lines, curves, shapes, and text. The basic syntax of the **`\draw`** command is as follows:

```latex
\draw[<options>] (<starting point>) -- (<ending point>);
```

### <options>

This is an optional argument that allows you to specify additional settings for the drawing. Options are provided within square brackets (**`[]`**), separated by commas. Some common options include:

- **`color`**: Specifies the color of the line or shape. For example, **`color=red`** sets the line color to red.
- **`line width`**: Sets the thickness of the line. For example, **`line width=1pt`** sets the line width to 1 point.
- **`dashed`**: Creates a dashed line.
- **`fill`**: Sets the fill color for shapes.
- **`draw`**: Specifies whether the shape should be drawn or not.

### <(starting and end point)>

These are the coordinates that define the starting and ending points of the line or shape. You can use absolute coordinates (e.g., **`(0,0)`**) or relative coordinates (e.g., **`(1,0)`** to move 1 unit to the right from the current position). The **`--`** symbol connects the starting and ending points with a line.