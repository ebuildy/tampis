## Dump config

```
 ./tampis ./example/helm-elk/config/prod.conf
```

## Build template

 ```
  ./tampis ./example/helm-elk/config/prod.conf ./example/helm-elk/value-template.yaml > ./example/helm-elk/build/values.yaml
```

## Build template certif

```
./tampis --config-path=elasticsearch.ingress.certif ./example/helm-elk/config/prod.conf ./example/helm-elk/certs-template.yaml > ./example/helm-elk/build/certif-elasticsearch.yaml

./tampis --config-path=kibana.ingress.certif ./example/helm-elk/config/prod.conf ./example/helm-elk/certs-template.yaml > ./example/helm-elk/build/certif-kibana.yaml
```
