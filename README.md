## Matlab Plotting Examples
#### Some examples for plotting different types of data

See `example_images/` for the outputs from these files (PNG). Note that publication-quality figures will usually require a vector graphics format (SVG/EPS/PDF) along with some manual editing to improve font clarity, etc. The examples shown here are in unedited raster format and are only meant to be illustrative.

##### Column data

From `example_data/column_data.txt`. Used with:

* `line_plot.m`: Standard line plot with different formatting options

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/line_plot.png)

* `stacked_area.m`: Stacked area plot with color options

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/stacked_area.png)

* `histogram_cdf.m`: Standard plots of frequency distributions

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/histogram_and_cdf.png)

* `parallel_coordinate.m`: Plots row entries as lines instead of columns. Options to scale all values between `[0,1]` and toggle solutions on/off above/below a certain threshold. (These functions are included in `/util/`).

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/parallel_coordinate.png)

##### Gridded 2D data

From `example_data/gridded_2D.txt`. Used with:

* `imagesc_plot.m`: Show matrix values directly as color blocks

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/imagesc_plot.png)

* `contour_surf.m`: Contour, filled contour, and surface plots of meshgrid data

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/contour_surf.png)

##### Non-Gridded 2D data (e.g. experimental data)

From `example_data/non_gridded_2D.txt`. The data file contains rows of `(x,y,z)` points that are not on a regular grid. Used with:

* `scatter_plot.m`: Plot the irregularly spaced points as dots, with `Z` values as the color

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/scatter_plot.png)

* `contourf_non_gridded.m`: Use Matlab's built-in `griddata` function to interpolate the data onto a standard meshgrid, which can then be used for standard contour/mesh/surf plots, etc.

![Image](https://raw.github.com/jdherman/matlab-plotting-examples/master/example_images/contourf_non_gridded.png)