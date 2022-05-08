# cmg-kubernetes-app

Packaging for CMG components to run as a single Kubernetes App

## TODO

### CMG Analytics

* store database schema in configmap
* ensure its service account can read config maps
* configure authentication user via secret
  * "CMG_PASSWORD"
  * "CMG_USER"
  * perhaps that should be "CMG_ANALYTICS_USER"?

### CMG

* use secret to connect to CMG Analytics
* add environment configuration for external services
* use secrets for external service API Token
* --Go in container optimization (processor: https://github.com/golang/go/issues/33803)--

### Overall

* Prometheus Metrics
* Micrometer Instrumentation
* Grafana Dashboard
* Prometheus Alertmanager Alerts
* build with Tekton
* mono repo with Bazel multi language build?