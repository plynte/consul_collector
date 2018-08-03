# consul_collector
BlueKing 蓝鲸监控 组件监控 自定义组件 consul采集器 Demo

# make a collector
> 以下内容基于蓝鲸监控1.4.62实践

1. download the [consul_exporter-0.3.0.linux-amd64.tar.gz](https://github.com/prometheus/consul_exporter/releases/download/v0.3.0/consul_exporter-0.3.0.linux-amd64.tar.gz)

2. run the exporter and get metrics
```bash
./consul_exporter
curl http://localhost:9107/metrics
```

3. configurate the file
```
├── config_schema.json
├── description.md
├── exporter.zip // step 4
├── info.json
├── logo.png
└── metrics.json
```

4.rename exporter and ZIP
```bash
mv consul_exporter exporter-linux
zip exporter.zip exporter-linux
```

