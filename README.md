# kube-prometheus-stack

``` shell
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update
# helm show values prometheus-community/kube-prometheus-stack --version 56.9.0 > values.default.yaml
helm upgrade --install kube-prometheus-stack prometheus-community/kube-prometheus-stack -n monitoring --create-namespace --version 56.9.0 -f values.yaml
````