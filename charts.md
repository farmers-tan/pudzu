# [charts.py](charts.py)

## Summary 
Pillow-based charting.
 
## Dependencies
*Required*: [pillow](http://pillow.readthedocs.io/en/4.2.x/index.html), [pandas](http://pandas.pydata.org/), [toolz](http://toolz.readthedocs.io/en/latest/index.html),  [bamboo](bamboo.md), [pillar](pillar.md), [utils](utils.md).

*Optional*: [dates](dates.md) (for flexible time charts and month charts).

## Documentation

Three chart types are currently supported: **bar charts**, **time charts** and **grid charts**. For usage information, see the docstrings and [sample scripts](dataviz/).

### Legends

**generate_legend**: generate a chart category legend.

![smurf etymology legend](images/chart_legend.png)

### Bar charts

**bar_chart**: generate a bar chart; supports grouped, stacked and percentage stacked charts, as well as horizontal charts and flexible coloring and labeling.

![uk elections bar chart](images/chart_elections.png)

![us elections bar chart](images/chart_uspopular.jpg)

### Time charts

**time_chart**: generate a time chart; supports numeric and date timelines highlighting both ranges and events.

![g7 time chart example](images/chart_g7.png)

![jerusalem time chart example](images/chart_jerusalem.jpg)

### Grid charts

**grid_chart**: generate an image grid chart; essentially a convenient wrapper for `Image.from_array`.

![grid chart example](images/chart_periodic.png)

![grid chart example](images/chart_markovtext.png)

### Map charts

**map_chart**: generate a map chart. Input is a map template with each region having a unique color. Regions can be named (see generate_name_csv), labelled (see generate_bbox_csv) and have overlays such as label arrows.

![map chart example](images/chart_femaleleaders.png)

![map chart example](images/chart_dishes.jpg)

### Calendar charts

**month_chart**: generate a calendar chart for a given month.

![jerusalem time chart example](images/chart_trump.jpg)
