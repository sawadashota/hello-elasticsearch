ping:
	curl http://127.0.0.1:9200/_cat/health
seed:
	http 'http://localhost:9200/bank/account/_bulk?pretty&refresh' @../fixture/accounts.json
setup-dashboards:
	docker-compose run --rm metricbeat setup --dashboards
module-list:
	docker-compose run --rm metricbeat ./metricbeat modules list
enable-docker:
	docker-compose run --rm metricbeat ./metricbeat modules enable docker
enable-system:
	docker-compose run --rm metricbeat ./metricbeat modules enable system
