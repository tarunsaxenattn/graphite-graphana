# Use the attached docker compose

# Help link
https://www.linode.com/docs/guides/install-graphite-and-grafana/

# Testing

1. Run a separate ubuntu container and install telegraf on it
2. Use the attached config
3. Edit config file and add graphite address
3. Restart telegraf 

```
root@8e0804174e43:/# telegraf --config /etc/telegraf/telegraf.conf
2022-01-29T08:39:57Z I! Starting Telegraf 1.14.3
2022-01-29T08:39:57Z I! Loaded inputs: kernel mem processes swap system cpu disk diskio
2022-01-29T08:39:57Z I! Loaded aggregators:
2022-01-29T08:39:57Z I! Loaded processors:
2022-01-29T08:39:57Z I! Loaded outputs: graphite
2022-01-29T08:39:57Z I! Tags enabled: host=8e0804174e43
2022-01-29T08:39:57Z I! [agent] Config: Interval:10s, Quiet:false, Hostname:"8e0804174e43", Flush Interval:10s


```

