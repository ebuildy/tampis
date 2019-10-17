# tampis

Convert data + template to string. data is coming from a HOCON file, template from Jinja format. My usecase is to build Helm values file from template and env'able config.

## Naming

``tampis`` from french word ``tant pis`` + ``template``

# Usage

## Print full configuration

```
./tampis ./components/conso/config/dev.conf
```

Usefull to understand file includes, merges etc...

## NEW option => "--config-path"

Allow to select a sub configuration tree

```
./tampis ./components/conso/config/dev.conf --config-path=elasticsearch.ingress.certif
```

## Templatize

```
./tampis ./components/conso/config/dev.conf ./components/conso/values-template.yaml > ./components/conso/values.yaml
```

## HOCON spec

https://github.com/lightbend/config/blob/master/HOCON.md
