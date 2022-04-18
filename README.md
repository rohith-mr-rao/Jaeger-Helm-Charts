# Jaeger-Helm-Charts

Elastic search is deployed in outside

helm install jaeger ../helm-charts \
  --set provisionDataStore.cassandra=false \
  --set storage.type=elasticsearch \
  --set storage.elasticsearch.host=redd-staging-hidd-staging.desaall.com \
  --set storage.elasticsearch.port=16180 \
  --set storage.elasticsearch.user=dafafdf\
  --set storage.elasticsearch.password=asfasdfsfd  \
  -n observability


kubectl port-forward -n  observability service/jaeger-query 9090:80

