# pgfplots

The **`\begin{axis}`** environment in **`pgfplots`** allows for various optional arguments that you can use to customize your plot. Here's the format with all the optional arguments listed:

```latex
\begin{axis}[
    % Axis labels and title
    title={Title},
    xlabel={X-label},
    ylabel={Y-label},
    zlabel={Z-label}, % For 3D plots

    % Axis limits
    xmin=value,
    xmax=value,
    ymin=value,
    ymax=value,
    zmin=value, % For 3D plots
    zmax=value, % For 3D plots

    % Ticks and tick labels
    xtick={list of positions},
    ytick={list of positions},
    ztick={list of positions}, % For 3D plots
    xticklabels={list of labels},
    yticklabels={list of labels},
    zticklabels={list of labels}, % For 3D plots
    xticklabel style={options},
    yticklabel style={options},
    zticklabel style={options}, % For 3D plots
    xtick align=value, % For horizontal placement of tick labels
    ytick align=value, % For horizontal placement of tick labels
    ztick align=value, % For 3D plots

    % Grid lines
    grid=type, % type: major, minor, both, none
    major grid style={options},
    minor grid style={options},
    xmajorgrids=value,
    ymajorgrids=value,
    zmajorgrids=value, % For 3D plots
    xminorgrids=value,
    yminorgrids=value,
    zminorgrids=value, % For 3D plots

    % Legend
    legend entries={list of entries},
    legend pos=position, % Position of the legend (north, south, east, west, etc.)
    legend style={options},

    % Plot styles and options
    width=value, % Width of the plot
    height=value, % Height of the plot
    domain=value, % Set the domain of the plot
    samples=value, % Number of samples to plot for the function
    color=value, % Line color
    mark=value, % Marker style (none, circle, square, etc.)
    mark options={options}, % Marker options
    only marks, % To plot only markers without lines
    smooth, % Smooths the plot
    ...

    % Other options
    scale only axis=value,
    clip=value,
    ...

    % Additional customizations
]
% Plot commands go here
\end{axis}
```

Please note that not all options listed above need to be used at once. You can select the ones that fit your specific plot requirements. Additionally, some options are specific to 3D plots, and you may ignore them if you are creating a 2D plot.

Remember to replace **`value`**, **`list of positions`**, **`list of labels`**, **`list of entries`**, and **`options`** with appropriate values or settings according to your data and preferences.

[Some Useful graph](<pgfplots/Some Useful graph .md>)