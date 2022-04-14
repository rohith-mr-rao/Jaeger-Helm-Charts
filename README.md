# Jaeger-Helm-Charts

Elastic search is deployed in outside

helm install install ../Jaeger-Helm-Charts  \
  --set provisionDataStore.cassandra=false \
  --set storage.type=elasticsearch \
  --set storage.elasticsearch.host=<HOST> \
  --set storage.elasticsearch.port=<PORT> \
  --set storage.elasticsearch.user=<USER> \
  --set storage.elasticsearch.password=<password>
