#### Exporter
> exporter可执行文件名称必须为: exporter-linux
> 上传文件必须打包为zip格式包

#### config_schema.json
定义运行prometheus exporter的配置项，如采集服务的访问方式（如redis账号）、metrics监听地址等
```json
[
    {
        "default": "http://127.0.0.1:9107/metrics",
        "mode": "collector",
        "type": "text",
        "name": "_exporter_url_",
        "description": "Consul指标采集器",
        "visible": false
    }
]
```
