# telegraf-influxdb-cloud-monitoring

# 🚀 Monitor linux system metrics using Telegraf collector and InfluxDB cloud 🚀

https://github.com/coding-to-music/telegraf-influxdb-cloud-monitoring

From / By https://docs.influxdata.com/influxdb/cloud/get-started/

https://docs.influxdata.com/influxdb/cloud/get-started/#add-sample-data-with-community-templates

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

Version: InfluxDB v2.3.0

Platform: Ubuntu & Debian

```
# influxdb.key GPG Fingerprint: 05CE15085FC09D18E99EFB22684A14CF2582E0C5
wget -q https://repos.influxdata.com/influxdb.key
echo '23a1c8836f0afc5ed24e0486339d7cc8f6790b83886c4c96995b88a061c5bb5d influxdb.key' | sha256sum -c && cat influxdb.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/influxdb.gpg > /dev/null
echo 'deb [signed-by=/etc/apt/trusted.gpg.d/influxdb.gpg] https://repos.influxdata.com/debian stable main' | sudo tee /etc/apt/sources.list.d/influxdata.list

sudo apt-get update && sudo apt-get install influxdb2
```

## Telegraf open source data collector

Telegraf is a plugin-driven server agent for collecting and sending metrics and events from databases, systems, and IoT sensors. Telegraf is written in Go and compiles into a single binary with no external dependencies, and requires a very minimal memory footprint.

With 200+ plugins already written by subject matter experts on the data in the community, it is easy to start collecting metrics from your endpoints.

Version: Telegraf v1.23.2

Platform: Docker Image

# Debian-based image

```
docker pull telegraf
```

## Install Telegraf - Platform: Ubuntu & Debian

Version: Telegraf v1.23.2

SHA256: a557d289fbe3058a784d4aacec2173276d4443b494117d7b31a8434a1926fe2b

```
# influxdb.key GPG Fingerprint: 05CE15085FC09D18E99EFB22684A14CF2582E0C5
wget -q https://repos.influxdata.com/influxdb.key
echo '23a1c8836f0afc5ed24e0486339d7cc8f6790b83886c4c96995b88a061c5bb5d influxdb.key' | sha256sum -c && cat influxdb.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/influxdb.gpg > /dev/null
echo 'deb [signed-by=/etc/apt/trusted.gpg.d/influxdb.gpg] https://repos.influxdata.com/debian stable main' | sudo tee /etc/apt/sources.list.d/influxdata.list
```

```
sudo apt-get update && sudo apt-get install telegraf
```

## 3. Start Telegraf

Finally, you can run the following command to start the Telegraf agent running on your machine.

```
telegraf --config https://eastus-1.azure.cloud2.influxdata.com/api/v2/telegrafs/07fcce8c53afd000
```

## IDE Extensions

InfluxData prides itself on its effort to prioritize developer happiness. This included providing developers with a variety of tools to interact with InfluxDB v2 OSS or InfluxDB Cloud, so they can pick the development style that works best for them. We're starting with the VS Code community.

Platform: Flux for Visual Studio Code

https://marketplace.visualstudio.com/items?itemName=influxdata.flux

## InfluxDB Cloud CLI

InfluxDB Cloud includes a command-line interface (CLI) for download. This CLI can be used to interact with your InfluxDB Cloud account.

Version: InfluxDB Cloud CLI v2.3.0

Platform: Ubuntu & Debian

```
# influxdb.key GPG Fingerprint: 05CE15085FC09D18E99EFB22684A14CF2582E0C5

wget -q https://repos.influxdata.com/influxdb.key
echo '23a1c8836f0afc5ed24e0486339d7cc8f6790b83886c4c96995b88a061c5bb5d influxdb.key' | sha256sum -c && cat influxdb.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/influxdb.gpg > /dev/null
echo 'deb [signed-by=/etc/apt/trusted.gpg.d/influxdb.gpg] https://repos.influxdata.com/debian stable main' | sudo tee /etc/apt/sources.list.d/influxdata.list

sudo apt-get update && sudo apt-get install influxdb2-cli
```

## 1. Install the Latest Telegraf

You can install the latest Telegraf by visiting the InfluxData Downloads page. If you already have Telegraf installed on your system, make sure it's up to date. You will need version 1.9.2 or higher.

## 2. Configure your API Token

Your API token is required for pushing data into InfluxDB. You can copy the following command to your terminal window to set an environment variable with your API token.

```
export INFLUX_TOKEN=<INFLUX_TOKEN>
```

## 3. Start Telegraf

Finally, you can run the following command to start the Telegraf agent running on your machine.

```
telegraf --config https://eastus-1.azure.cloud2.influxdata.com/api/v2/telegrafs/07fcce8c53afd000
```

## Stop InfluxDB and Telegraf from running

```
sudo netstat -nlp

sudo systemctl status

sudo systemctl status influxdb
sudo systemctl stop influxdb
sudo systemctl disable influxdb

sudo systemctl status telegraf
sudo systemctl disable telegraf
```
