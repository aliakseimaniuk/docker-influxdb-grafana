# Docker-compose for InfluxDB and Grafana

Docker-compose for InfluxDB and Grafana

## Tools

* [Grafana](https://grafana.com/) allows you to query, visualize, alert on and understand your metrics no matter where they are stored. Create, explore, and share dashboards with your team and foster a data driven culture.
* [InfluxDb](https://www.influxdata.com/) is an open-source time series database developed by InfluxData. It is written in Go and optimized for fast, high-availability storage and retrieval of time series data in fields such as operations monitoring, application metrics, Internet of Things sensor data, and real-time analytics. It also has support for processing data from Graphite.
* [Chronograf](https://www.influxdata.com/time-series-platform/chronograf/) is the user interface component of InfluxData’s TICK Stack. It allows you to quickly see the data that you have stored in InfluxDB so you can build robust queries and alerts. It is simple to use and includes templates and libraries to allow you to rapidly build dashboards with real-time visualizations of your data.
* [Docker](https://www.docker.com/)  is a computer program that performs operating-system-level virtualization also known as containerization.

## Installation instructions

1. Clone repository

``` powershell
git clone https://github.com/aliakseimaniuk/docker-influxdb-grafana.git
```

1. Open folder with downloaded source code in powershell/terminal/cmd
1. Run the following command

``` powershell
docker-compose up -d
```

> Use [Compose command-line reference](https://docs.docker.com/compose/reference/) for more information about compose commands.

### Advanced setup

If you want to use existing Grafana or InfluxDb data you need to do the following:

#### InfluxDb

1. Open folder with source code in file explorer.
1. Create `influxdb/data` or `influxdb/config` folders in the root of the project and copy `data` or `config` folder from existing InfluxDb.

#### Grafana

1. Open folder with source code in file explorer.
1. Create `grafana/data` folder in the root of the project and copy `data` folder from existing Grafana.

> See [docker-compose.yml](./docker-compose.yml) for more information.

## Check the installation

1. Grafana's url: [http://localhost:3000](http://localhost:3000)
1. Chronograf's url: [http://localhost:8888](http://localhost:8888)
