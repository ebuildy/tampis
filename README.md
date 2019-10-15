# tampis

Convert data + template to string. data is coming from a HOCON file, template from Jinja format.

# Usage

## Print full configuration

```
./tampis ./components/conso/config/dev.conf
```

Usefull to understand file includes, merges etc...

## Templatize

```
./tampis ./components/conso/config/dev.conf ./components/conso/values-template.yaml > ./components/conso/values.yaml
```

## HOCON spec

https://github.com/lightbend/config/blob/master/HOCON.md

# Naming

``tampis`` from french word ``tant pis`` + ``template``
