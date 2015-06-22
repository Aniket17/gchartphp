# gChartPhp #

### Project migration ###
The project was migrated to GitHub, since we cannot actively administer this project any longer.  You can access the main project [here](https://github.com/pacbard/gChartPhp).  The project will continue to be mirrored on this Google Code page.

Use the master branch for stable releases, the experimental branch for the development release, and the legacy branch for the old release of the wrapper (this branch will not be actively updated).

### PHP Object wrapper for the Google Chart API ###

A simple PHP Object wrapper for the [Google Chart API](http://code.google.com/apis/chart/image_charts.html). Should help anyone who needs to automate the building of the Google Chart url. Supports (almost) all types of charts.

Get the code here: [code link](http://gchartphp.googlecode.com/svn/trunk/)

## Prerequisites ##
To use this API, you should have a little PHP experience; a little patience to read the documentation; and a little persistence to keep trying if your first charts don't look as you expect them to.

## Pie Chart Example ##
![http://chart.apis.google.com/chart?cht=p&chs=350x200&chd=t:112,315,66,40&chdl=first|second|third|fourth&chco=ff3344,11ff11,22aacc,3333aa&chl=first|second|third|fourth&image.png](http://chart.apis.google.com/chart?cht=p&chs=350x200&chd=t:112,315,66,40&chdl=first|second|third|fourth&chco=ff3344,11ff11,22aacc,3333aa&chl=first|second|third|fourth&image.png)

pie chart using the gPieChart class.

code:
```
$piChart = new gPieChart();
$piChart->addDataSet(array(112,315,66,40));
$piChart->setLabels = array("first", "second", "third","fourth");
$piChart->setLegend(array("first", "second", "third","fourth"));
$piChart->setColors = array("ff3344", "11ff11", "22aacc", "3333aa");

```

Check out the [Examples](Examples.md)

## Additional Documentation ##

Documentation is available for the following options:
  * [ChartSize](ChartSize.md)
  * [Axes](Axes.md)
  * [DataEncoding](DataEncoding.md)

## Notes ##

Welcome **bardellie**, who has taken over active development of gChartPhp

I am pleased with how the code is shaping up. I haven’t had much of an opportunity in the past to play with inheritence and polymorphism in PHP.