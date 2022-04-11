# Simple Ruby Helm Chart

This is a simple Helm chart to deploy [Simple Ruby Server](https://github.com/salareinavipour/http_server).

## Getting started

Install `Helm 3` and then deploy this app with:

```
helm install simple-ruby . --values values.yaml
```

## Attention

Be aware of these things:
- I assumed that you're using `Nginx Ingress Controller`.
- If you want to deploy it on `Minikube`, make sure to first build the image in [Simple Ruby Server](https://github.com/salareinavipour/http_server) and tag it according to the chart values and then load it to `Minikube` using:

```
minikube image load ruby_server:<tag>
```