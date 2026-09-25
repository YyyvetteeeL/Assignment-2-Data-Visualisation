# Process

<!-- Same as assignment 1, same honesty. Which tools you used and for what; one
thing you kept and why it was good; one thing you rejected and why it was wrong.
"I did not use any" is fine if it is true.

If a model wrote most of plot.py, which is likely and allowed, the interesting part
is what you had to correct: did it invent a column name, use pandas where a list
would do, silently drop the rows it could not parse? -->

## 9.17
1.I initially wanted to choose a typhoon because it is related to one of my visual novels. However, I realized that I didn’t have any particularly interesting ideas for visualizing typhoon data. After some thought, I decided to drop the typhoon idea and choose something that inspired me more: a heavy rainstorm across the whole of Hong Kong.
2.I then chose a Hong Kong rainstorm to explore how rainfall changes across space and time.I selected the 18 June 2026 rainstorm and decided to investigate its historical gridded data.

## 9.24
1.I collected the gridded rainfall nowcast data for the whole day of June 18, with data available every 15 minutes. I inspected the data to understand how the rainfall changed across Hong Kong throughout the day.
2.However, using all the data would create too many frames. After comparing the rainfall patterns, I decided to focus on the more active period from 06:00 to 12:00 and use a 30-minute interval, keeping the visualisation manageable while still showing the changes over time.

## 9.25
I created a first visualisation using latitude and longitude as spatial positions and rainfall intensity as colour. The result showed clear rainfall patterns across the grid, but the large spatial range made Hong Kong itself difficult to identify.

Visual Performance Tuning, You can see the results of several debugging runs in "out".
1.I first mapped rainfall onto a scatter plot, but it looked too much like a conventional data chart.
2.I tested a grid-based rainfall field, but it looked like a typical weather heatmap and felt too rigid.
3.I changed the data points into particles and mapped rainfall to their size and intensity, but the initial particles were too sparse.
4.I experimented with a dark background for a more atmospheric effect. I later switched to a light background for better clarity.
5.OMG Some particles appeared to contain smaller circles. I found that multiple forecast values were being plotted at the same location.
6.I kept one forecast value per location and refined the particle field. Higher rainfall now appears as larger and darker particles.


## Tools

## Kept

## Rejected
