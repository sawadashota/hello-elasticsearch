ping:
	curl http://127.0.0.1:9200/_cat/health
seed:
	http 'http://localhost:9200/bank/account/_bulk?pretty&refresh' @../fixture/accounts.json
