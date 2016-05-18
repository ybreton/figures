# figures
*MATLAB functions for non-default figure types and overlays*

Adds figure types, overlays, and elements to MATLAB.

* barerrorbar
   * [bh,eh,ch] = barerrorbar(x,y,l,u,*'property'*,*value*)
   
   returns the bar handles (bh), error handles (eh), and patch child object handles (ch) along with a bar graphs with specified x data,
   y data, lower bounds, and upper bounds.
   
* barerrorbarXY
   * [xBar,yBar] = barerrorbarXY(ch,*'property'*,*value*)
   
   Support function for barerrorbar. Returns the center x location and top y location of each bar in bar handles ch.
   
* barSEM
   * [bh,eh] = barSEM(m,s,*'property'*,*value*)
   
   Produces a bar graph with means m and standard errors s.
   
* box_whisker_plot
   * [ph,stats] = box_whisker_plot('x',x,'data',data,*'property'*,*value*)
   
   Produces a nicer box-whisker plot than the default boxplot.
   
* dockAllFigures
   * dockAllFigures(h,sortFigs,*'property'*,*value*)
   
   Docks all open figures, for organizational purposes. Figures can optionally be specified with h, and can optionally be sorted 
   when docked with flag sortFigs.
   
* figureFontSizes
   * status = figureFontSizes(fn,*'property'*,*value*)
   
   Automatically re-sizes the fonts of figures fn.
   
* high_low_close_plot
   * handles = high_low_close_plot(x,hi,lo,cl,*'property'*,*value*)
   
   Produces a stock-like high-low-close plot.
   
* HighLowPatch
   * h = HighLowPatch(X,H,L,*'property'*,*value*)
   
   Produces a high-low plot with filled colored patches
   
* plot_grouped_Y
   * [ph,eh,ah,fh] = plot_grouped_Y(X,Y,*'property'*,*value*)
   
   Plots the mean and spread (user-defined) of Y for each unique value of x.
   
* plotBoxOverlay
   oh = plotBoxOverlay(y,*'property'*,*value*)
   
   Plots a raw data y (by column or with X-axis center locations indicated) overlay, where points that would be included in the same
   histogram bin are aligned horizontally at their y locations, in a manner that minimizes any cognitive bias when viewed.
   
* plotSignificant
   * th = plotSignificant(c)
   
   Indicates significantly different groups according to MATLAB's *multcompare* output c.
   
* removeBoxplotXtick
   * flag = removeBoxplotXtick(fh)
   
   Removes hanging ticks when boxplots are produced in MATLAB.
   
* sortFigFiles
   * sortFigFiles(*fd*)
   
   Sorts figure files in current or specified directory fd into subdirectories based on figure file extension.
   
* step_through_figures
   * step_through_figures(*'property'*,*value*)
   
   Allows user to step through all figures in directory one at a time.
   
* trendline
   * h=trendline(x,y,*'property'*,*value*)
   
   Adds a trend line to the data (x,y).
   
* undockAllFigures
   * undockAllFigures(*h*,*sortFigs*)
   
   Complement to dockAllFigures, takes all figures or those in h and undocks them to new figure windows. Flag sortFigs can optionally
   produce the windows in sorted order.
   
* xticklabelf
   * h = xticklabelf(labels,*'property'*,*value*)
   
   Formatted xticklabel, much like sprintf for x-ticks.
   
* yticklabelf
   * h = yticklabelf(labels,*'property'*,*value*)
   
   Formatted yticklabel, much like sprintf for y-ticks.

