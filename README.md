# STAT442-Assignment-10
Assignment 10 for my STAT 442 class.

For this assignment we updated our Assignment 9 Shiny app.

Changes in update:  
1) Added a tab for us map showing fatalities (filter independent of original tab)
2) Changed background and plot colors
3) Added notes at bottom of app with creator names and sources.

This app uses data pulled from https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars
and displays it in a way that is more usable to the average consumer. 

Our app has two tabs; one for accidents and one for fatalities.

The accidents tab allows you to filter by month and by state, and view the time of day that accidents happened (bar plot) 
and the lighting conditions during the accident (pie plot).

The fatalities tab allows you to filter by month (independently of the accidents tab, the two filters are not linked) and
view the fatalities by state (us map plot). 

A note about the us map plot: Because of how the library usmap in written, us map plots do not scale well with window size 
changes. We scaled it to the best of our ability to look well at fullscreen, but it is still somewhat hard to read. 
Updating a us map plot dynamically also takes a noticable amount of time, likely do to some ineffeciency in how the library is coded and
how that code interacts with the dynamically changing filters of the Shiny app.
