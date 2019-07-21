# ChartBars
Simple chart bars for incorporation e.g. into google sheet cells

Example:

To chart a value 0 to 1 in Google Sheets, scale it to 0-100, round to integer, and build into an URL:

=image("https://rsargent.github.io/ChartBars/bars/green/" & round(D8*100) & ".png", 2)

Second arg to image is "2" -- mode for reshape image to exactly match cell size
