# Jobber

1. [Shared library](https://github.com/FranciscoJavierMartin/jobber-shared)
2. [Notifaction](https://github.com/FranciscoJavierMartin/jobber-notification)

How to set password for kibana
```sh
curl -s -X POST -u elastic:admin1234 -H "Content-Type: application/json" http://localhost:9200/_security/user/kibana_system/_password -d "{\"password\":\"kibana\"}"
```

How to create token for kibana
```sh
bin/elasticsearch-service-tokens create elastic/kibana jobber-kibana
```