# fl_animated_linechart

[![Codemagic build status](https://api.codemagic.io/apps/5d5e513ff8278e001ca52adf/5d5e513ff8278e001ca52ade/status_badge.svg)](https://codemagic.io/apps/5d5e513ff8278e001ca52adf/5d5e513ff8278e001ca52ade/latest_build)

![Animations](chart.gif)

An animated linechart library for flutter.
 - Support for datetime xaxis
 - highlight selection
 - animation the chart

## Getting Started

Try the sample project or include in your project.

![Chart example with highlight](withSelection.png)


![Area Chart example](areaChart.png)


Example code:

    LineChart lineChart = LineChart.fromDateTimeMaps([line1, line2], [Colors.green, Colors.blue]);

    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title),
      ),
      body: Container(
        child: Column(
            mainAxisSize: MainAxisSize.max,
            mainAxisAlignment: MainAxisAlignment.spaceBetween,
            crossAxisAlignment: CrossAxisAlignment.stretch,
            children: [
              Expanded(child: AnimatedLineChart(lineChart)),
            ]
        ),
      ),
    );

![Example app](exampleScreenshot.png)
