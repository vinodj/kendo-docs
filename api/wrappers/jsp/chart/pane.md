---
title: chart-pane
slug: jsp-chart-pane
tags: api, java
publish: true
---

# \<kendo:chart-pane\>
A JSP tag representing Kendo Pane.

#### Example
    <kendo:chart-panes>
        <kendo:chart-pane></kendo:chart-pane>
    </kendo:chart-panes>


## Configuration Attributes


### name `String`

The unique pane name.

#### Example
    <kendo:chart-pane name="name">
    </kendo:chart-pane>



### margin `float`

The margin of the pane.

#### Example
    <kendo:chart-pane margin="margin">
    </kendo:chart-pane>



### padding `float`

The padding of the pane.

#### Example
    <kendo:chart-pane padding="padding">
    </kendo:chart-pane>



### background `String`

The background color of the pane.

#### Example
    <kendo:chart-pane background="background">
    </kendo:chart-pane>



### height `float`

The pane height in pixels.

#### Example
    <kendo:chart-pane height="height">
    </kendo:chart-pane>



### title `String`

The pane title text or configuration. Further configuration is available via [kendo:chart-pane-title](#kendo-chart-pane-title). 

#### Example
    <kendo:chart-pane title="title">
    </kendo:chart-pane>



## Child JSP Tags

### kendo:chart-pane-border

The border of the pane.

More documentation is available at [kendo:chart-pane-border](/api/wrappers/jsp/chart/pane-border).

#### Example

    <kendo:chart-pane>
        <kendo:chart-pane-border></kendo:chart-pane-border>
    </kendo:chart-pane>
 
### kendo:chart-pane-title

The pane title text or configuration.

More documentation is available at [kendo:chart-pane-title](/api/wrappers/jsp/chart/pane-title).

#### Example

    <kendo:chart-pane>
        <kendo:chart-pane-title></kendo:chart-pane-title>
    </kendo:chart-pane>
 
