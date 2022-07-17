# telegraf-influxdb-cloud-monitoring

# 🚀 Monitor linux system metrics using Telegraf collector and InfluxDB cloud 🚀

https://github.com/coding-to-music/telegraf-influxdb-cloud-monitoring

From / By

https://portal.influxdata.com/downloads/

## Environment variables:

```java

```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/telegraf-influxdb-cloud-monitoring.git
git push -u origin main
```

# Install InfluxDB and Telegraf

https://portal.influxdata.com/downloads/

## Install Influx Docker

```
docker pull influxdb:2.3.0
```

This version is ready for Docker upgrade from 1.x to 2.x. See docs: https://docs.influxdata.com/influxdb/v2.0/upgrade/v1-to-v2/docker

3. Start Telegraf
   Finally, you can run the following command to start the Telegraf agent running on your machine.

telegraf --config https://eastus-1.azure.cloud2.influxdata.com/api/v2/telegrafs/07fcce8c53afd000

InfluxDB 2.x Open Source

The next generation of InfluxDB is here

Check out the Getting Started guide

Want it hosted? Sign-up for InfluxDB Cloud. Get Started

InfluxDB 2.x Open Source Time Series Database

InfluxDB is an open source time series database. It has everything you need from a time series platform in a single binary – a multi-tenanted time series database, UI and dashboarding tools, background processing and monitoring agent. All this makes deployment and setup a breeze and easier to secure.

The InfluxDB Platform also includes APIs, tools, and an ecosystem that includes 10 client and server libraries, Telegraf plugins, visualization integrations with Grafana, Google Data Studio, and data sources integrations with Google Bigtable, BigQuery, and more.

Version: InfluxDB v2.3.0
Platform: Docker Image

```
docker pull influxdb:2.3.0
```

This version is ready for Docker upgrade from 1.x to 2.x. See docs: https://docs.influxdata.com/influxdb/v2.0/upgrade/v1-to-v2/docker

Documentation Release Notes

Version

InfluxDB v2.3.0

Platform: Ubuntu & Debian

# influxdb.key GPG Fingerprint: 05CE15085FC09D18E99EFB22684A14CF2582E0C5

wget -q https://repos.influxdata.com/influxdb.key
echo '23a1c8836f0afc5ed24e0486339d7cc8f6790b83886c4c96995b88a061c5bb5d influxdb.key' | sha256sum -c && cat influxdb.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/influxdb.gpg > /dev/null
echo 'deb [signed-by=/etc/apt/trusted.gpg.d/influxdb.gpg] https://repos.influxdata.com/debian stable main' | sudo tee /etc/apt/sources.list.d/influxdata.list

sudo apt-get update && sudo apt-get install influxdb2

Telegraf open source data collector
Telegraf is a plugin-driven server agent for collecting and sending metrics and events from databases, systems, and IoT sensors. Telegraf is written in Go and compiles into a single binary with no external dependencies, and requires a very minimal memory footprint.

With 200+ plugins already written by subject matter experts on the data in the community, it is easy to start collecting metrics from your endpoints.

For additional architecture (e.g. i386, riscv64, etc.) and operating system (e.g BSD, etc.) downloads please see the Telegraf GitHub Releases page.

Version

Telegraf v1.23.2
Platform

Docker Image

# Debian-based image

docker pull telegraf

# Alpine-based image

docker pull telegraf:alpine
Documentation Release Notes
IDE Extensions
InfluxData prides itself on its effort to prioritize developer happiness. This included providing developers with a variety of tools to interact with InfluxDB v2 OSS or InfluxDB Cloud, so they can pick the development style that works best for them. We're starting with the VS Code community.

Platform

Flux for Visual Studio Code
https://marketplace.visualstudio.com/items?itemName=influxdata.flux
Documentation

InfluxDB Cloud CLI

InfluxDB Cloud includes a command-line interface (CLI) for download. This CLI can be used to interact with your InfluxDB Cloud account.

Version: InfluxDB Cloud CLI v2.3.0

Platform: Ubuntu & Debian

influxdb.key GPG Fingerprint: 05CE15085FC09D18E99EFB22684A14CF2582E0C5

wget -q https://repos.influxdata.com/influxdb.key
echo '23a1c8836f0afc5ed24e0486339d7cc8f6790b83886c4c96995b88a061c5bb5d influxdb.key' | sha256sum -c && cat influxdb.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/influxdb.gpg > /dev/null
echo 'deb [signed-by=/etc/apt/trusted.gpg.d/influxdb.gpg] https://repos.influxdata.com/debian stable main' | sudo tee /etc/apt/sources.list.d/influxdata.list

sudo apt-get update && sudo apt-get install influxdb2-cli
