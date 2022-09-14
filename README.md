# exporter manager

## feature

batch exporter management
- start / stop
- batch start (max 10000) and batch stop
- metrics data size control
- connect pushgateway / prometheus

## design

- server
  - manage exporter
  - supply some metrics

- tool
  - cmd: start / stop exporter

- db
  - record exporter info (id, status, port)

## config

```yaml
exporter:
  group_one:
    count: 1000
    port_start: 10000
  group_two:
    count: 100
    port_start: 20000
mysql:
  host: localhost
  port: 3306
  user: root
  password: pwd
```

## build

## run
