---
title: chart-xAxisItem
slug: jsp-chart-xAxisItem
tags: api, java
publish: true
---

# \<kendo:chart-xAxisItem\>
A JSP tag representing Kendo XAxisItem.

#### Example
    <kendo:chart-xAxis>
        <kendo:chart-xAxisItem></kendo:chart-xAxisItem>
    </kendo:chart-xAxis>


## Configuration Attributes


### color `String`

Color to apply to all axis elements.
Individual color settings for line and labels take priority. Any valid CSS color string will work here, including hex and rgb.

#### Example
    <kendo:chart-xAxisItem color="color">
    </kendo:chart-xAxisItem>



### type `String`

The axis type.

#### Example
    <kendo:chart-xAxisItem type="type">
    </kendo:chart-xAxisItem>



### baseUnit `String`

The base time interval for the axis labels.
The default baseUnit is determined automatically from the value range. Available options:

#### Example
    <kendo:chart-xAxisItem baseUnit="baseUnit">
    </kendo:chart-xAxisItem>



### majorUnit `float`

The interval between major divisions in base units.

#### Example
    <kendo:chart-xAxisItem majorUnit="majorUnit">
    </kendo:chart-xAxisItem>



### max `Object`

The end date of the axis.
This is often used in combination with the

#### Example
    <kendo:chart-xAxisItem max="max">
    </kendo:chart-xAxisItem>



### min `Object`

The maximum value of the axis.
This is often used in combination with the

#### Example
    <kendo:chart-xAxisItem min="min">
    </kendo:chart-xAxisItem>



### minorUnit `float`

The interval between minor divisions in base units.
It defaults to 1/5th of the majorUnit.

#### Example
    <kendo:chart-xAxisItem minorUnit="minorUnit">
    </kendo:chart-xAxisItem>



### name `Object`

The unique axis name.

#### Example
    <kendo:chart-xAxisItem name="name">
    </kendo:chart-xAxisItem>



### narrowRange `boolean`

Prevents the automatic axis range from snapping to 0.

#### Example
    <kendo:chart-xAxisItem narrowRange="narrowRange">
    </kendo:chart-xAxisItem>



### pane `String`

The name of the pane that the axis should be rendered in.
The axis will be rendered in the first (default) pane if not set.

#### Example
    <kendo:chart-xAxisItem pane="pane">
    </kendo:chart-xAxisItem>



### reverse `boolean`

Reverses the axis direction -
values increase from right to left and from top to bottom.

#### Example
    <kendo:chart-xAxisItem reverse="reverse">
    </kendo:chart-xAxisItem>



### visible `boolean`

The visibility of the axis.

#### Example
    <kendo:chart-xAxisItem visible="visible">
    </kendo:chart-xAxisItem>



### axisCrossingValue `Object`

Value at which the Y axis crosses this axis. (Only for object)

#### Example
    <kendo:chart-xAxisItem axisCrossingValue="axisCrossingValue">
    </kendo:chart-xAxisItem>



## Child JSP Tags

### kendo:chart-xAxisItem-labels

Configures the axis labels.

More documentation is available at [kendo:chart-xAxisItem-labels](/api/wrappers/jsp/chart/xaxisitem-labels).

#### Example

    <kendo:chart-xAxisItem>
        <kendo:chart-xAxisItem-labels></kendo:chart-xAxisItem-labels>
    </kendo:chart-xAxisItem>
 
### kendo:chart-xAxisItem-line

Configures the axis line. This will also affect the major and minor ticks, but not the grid lines.

More documentation is available at [kendo:chart-xAxisItem-line](/api/wrappers/jsp/chart/xaxisitem-line).

#### Example

    <kendo:chart-xAxisItem>
        <kendo:chart-xAxisItem-line></kendo:chart-xAxisItem-line>
    </kendo:chart-xAxisItem>
 
### kendo:chart-xAxisItem-majorGridLines

Configures the major grid lines. These are the lines that are an extension of the major ticks through the
body of the chart.

More documentation is available at [kendo:chart-xAxisItem-majorGridLines](/api/wrappers/jsp/chart/xaxisitem-majorgridlines).

#### Example

    <kendo:chart-xAxisItem>
        <kendo:chart-xAxisItem-majorGridLines></kendo:chart-xAxisItem-majorGridLines>
    </kendo:chart-xAxisItem>
 
### kendo:chart-xAxisItem-majorTicks

The major ticks of the axis.

More documentation is available at [kendo:chart-xAxisItem-majorTicks](/api/wrappers/jsp/chart/xaxisitem-majorticks).

#### Example

    <kendo:chart-xAxisItem>
        <kendo:chart-xAxisItem-majorTicks></kendo:chart-xAxisItem-majorTicks>
    </kendo:chart-xAxisItem>
 
### kendo:chart-xAxisItem-plotBands

The plot bands of the xAxis.

More documentation is available at [kendo:chart-xAxisItem-plotBands](/api/wrappers/jsp/chart/xaxisitem-plotbands).

#### Example

    <kendo:chart-xAxisItem>
        <kendo:chart-xAxisItem-plotBands></kendo:chart-xAxisItem-plotBands>
    </kendo:chart-xAxisItem>
 
### kendo:chart-xAxisItem-title

The title of the value axis.

More documentation is available at [kendo:chart-xAxisItem-title](/api/wrappers/jsp/chart/xaxisitem-title).

#### Example

    <kendo:chart-xAxisItem>
        <kendo:chart-xAxisItem-title></kendo:chart-xAxisItem-title>
    </kendo:chart-xAxisItem>
 
