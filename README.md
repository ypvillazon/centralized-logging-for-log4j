# Logs centralization with Telegraf, InfluxDB and Grafana (unfinished)

This tutorial shows how you can centralize and track the logs of our applications easily and without much effort. Although it works for any type of logs, we will focus on the logs that are generated by default in Spring Boot.

## Let's install the tools

### Telegraf

Telegraf is a plugin-driven server agent for collecting & reporting metrics, and is the first piece of the TICK stack. ... It also has output plugins to send metrics to a variety of other datastores, services, and message queues, including InfluxDB, Graphite, OpenTSDB, Datadog, Librato, Kafka, MQTT, NSQ, and many others.

```bash
$ wget https://dl.influxdata.com/telegraf/releases/telegraf_1.13.3-1_amd64.deb
$ sudo dpkg -i telegraf_1.13.3-1_amd64.deb
```

Once the collector is installed, we will make the settings.