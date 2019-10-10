# tampis

Helm sub-charts much better! templatize sub-charts values.yaml file.

# File structure

```
examples/elk
├── Chart.yaml
├── charts
│   ├── elasticsearch-7.4.0.tgz
│   └── kibana-7.4.0.tgz
├── config # Configuration used by tampis
│   ├── dev # env name
│   │   └── data.yaml
│   └── prod # another env
│       └── data.yaml
├── requirements.lock
├── requirements.yaml # define deps as usually
├── values # define deps values, as template
│   ├── elasticsearch.yaml
│   └── kibana.yaml
├── values-dev.yaml # generated values
└── values-prod.yaml
```

# Usage

Respect file structure, then run ``tampis ./examples/elk``, this will generate ``values-{{env}}.yaml`` files. Then, use this chart as an usual Helm chart.
