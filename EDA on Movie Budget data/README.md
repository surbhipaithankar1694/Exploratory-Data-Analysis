## Objective

The file movie_budgets.txtcontains data on the budgets of 5,183 movies from 1906 to 2005, along with their lengths in minutes.
We wish to study log10(budget) as the response variable and year and length as explanatories.  
Note that these movies are not a representative sample of all movies, so we're not trying to generalize, only describe the data we have.

1. Using loess or otherwise, fit a model to predict log10(budget) from year and length. For simplicity, do not transform year and length (even though a transformation of length would probably be sensible.) We have to make a number of modeling choices:

- Should you fit a linear or curved function for year?  
- Should you fit a linear or curved function for length?  
- Do you need an interaction between year and length?  
- What span should you use in your loess smoother?  
- Should you fit using least squares or a robust fit?  

Some of these choices are clear-cut, while others will be a matter of preference.

2. Draw ONE set of faceted plots to display the fit -- either condition on year or length, whichever seems to you to be more interesting.
3. Draw a raster-and-contour plot (or other "3D" plot of your choice) to further display the fit. 

Please read the report for detailed analysis.
