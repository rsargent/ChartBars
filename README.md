# ChartBars
Simple chart bars for incorporation e.g. into google sheet cells

Example:

To chart a value 0 to 1 in Google Sheets, scale it to 0-100, round to integer, and build into an URL:

=image("https://rsargent.github.io/ChartBars/bars/green/" & min(100, round(D8*100)) & ".png", 2)

Second arg to image is "2" -- mode for reshape image to exactly match cell size

A more complicated example that charts number of steps taken from 0 to 15000, using red for less than 5000 steps, yellow for 5000-10000, and green for 10000+: 

=image("https://rsargent.github.io/ChartBars/bars/" & IFS(D8 < 5000, "red", D8 < 10000, "gold", TRUE, "green") & "/" & min(100, round((D8/15000)*100)) & ".png", 2)

Available colors:

* red
* orange
* gold
* yellow
* green
* cyan
* blue
* indigo
* magenta
* violet
* white
* grey
* black
