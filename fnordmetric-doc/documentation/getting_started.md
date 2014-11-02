Getting Started with FnordMetric
================================

FnordMetric is a framework for visualizing and collecting (timeseries) data
using SQL. It extends standard SQL with ChartSQL, allowing you to write queries
that return charts rather than tables. The query results are rendered as SVG
vector graphics or images.

The charts can easily be embedded into any website and customized using CSS.
This enables you to build beautiful dashboards within minutes using nothing
else than SQL.

---

_FnordMetric ships two binaries, each with it's own usecase:_

### fnordmetric-cli

fnordmetric-cli is probably best described as gnuplot meets SQL. It allows you
to run ChartSQL queries from the command line against external data sources,
like MySQL databases or CSV files.

Use fnordmetric-cli if you have already collected the source data and just
want to visualize it using ChartSQL.

[Getting started with fnordmetric-cli](/documentation/getting_started/fnordmetric-cli)
<br style="line-height:30px;"/>

### fnordmetric-server

fnordmetric-server is a standalone HTTP server application. It exposes a web UI
and a HTTP API to run ChartSQL queries. The query results are returned as JSON,
SVG or PNG.

Like fnordmetric-cli, the server allows you to execute queries against a number
of external backends like MySQL databases or CSV files. Additionally, the server
includes a facility to collect timeseries data and store them either on local
disk or in external storage (MySQL, HBase).

You can use fnordmetric-server as a one-stop solution for metric collection and
charting. Since fnordmetric-server aims to be a StatsD+graphite competitor, it
implements a wire compatible StatsD API.

[Getting started with fnordmetric-server](/documentation/getting_started/fnordmetric-server)




---

_Additionally, there are a number of client libraries for FnordMetric:_


### FnordMetric for HTML5

Plug fnordmetric charts into any website and build beautiful dashboards within
minutes using only SQL and HTML/CSS. Includes generic dashboard control elements.

[Getting started with the HTML5 API](/documentation/getting_started/fnordmetric-server)

### FnordMetric for JavaScript and node.js

The JavaScript client allows you to plug fnordmetric charts into any web
application. It also includes helper code to collect counters/timerseries
data in your node.js backend and send them to fnordmetric-server.

[Getting started with the JavaScript API](/documentation/getting_started/fnordmetric-server)

### FnordMetric for Ruby (on Rails)

The ruby client allows you to plug fnordmetric charts into an Ruby (on Rails)
web application. It also includes helper classes to collect counters/timerseries
data and send them to fnordmetric-server.

[Getting started with the ruby API](/documentation/getting_started/fnordmetric-server)




---

_FnordMetric also includes a number pre-built agents to collect data from common sources:_

### FnordMetric Community Contributed Agents

  + Docker Agent (fm-docker-agent)