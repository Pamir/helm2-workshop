```yaml
dependencies:

  - name: kube-state-metrics
    version: 2.0.*
    repository: https://kubernetes-charts.storage.googleapis.com/
    condition: kubeStateMetrics.enabled

  - name: prometheus-node-exporter
    version: 1.5.*
    repository: https://kubernetes-charts.storage.googleapis.com/
    condition: nodeExporter.enabled

  - name: grafana
    version: 3.5.*
    repository: https://kubernetes-charts.storage.googleapis.com/
    condition: grafana.enabled
```
```sh
helm dependency update .
ls -lart charts
```