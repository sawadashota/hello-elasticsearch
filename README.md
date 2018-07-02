Elasticsearch Hands on
===

[Basic](./basic)
---

Simple cluster

```shell-session
$ docker-compose up -d
```

[With Kibana](./kibana)
---

Add Kibana

```shell-session
$ docker-compose up -d
$ open http://localhost:5601/
```

[With metricbeat](./metricbeat)
---

Add metricbeat

```shell-session
$ docker-compose up -d

$ docker-compose run --rm metricbeat ./metricbeat modules enable docker system
$ docker-compose run --rm metricbeat setup --dashboards

$ open http://localhost:5601/
```
