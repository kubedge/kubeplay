# kubeplay

KUDEDGE Platform Play Server. Simple example of a project deployable on KUBEDGE.

## KUBEDGE Platform

Documentation is available [Here](http://kubedge.cloud) or [Here](https://kubedge.github.io)

## Main tutorials

- Docker image creation.
- Helm chart for Kubernetes deployment.
- Minimal size container build around GO binary.
- Multi architecture handling (AMD64 and ARM32V7).

## Related tutorials

- GITHUB as code.
- GERRITUB for code review.
- TRAVIS as CI.
- DOCKERHUB for image repository.

## Branch descrption

### master

Development and Deployment on KUBEDGE SDK. No Helm chart.

```bash
cd charts/kubeplay && helm install kubeplay . --values values.yaml --values values-dev.yaml
```

### arm32v7

Deployment on KUBEDGE Raspberry PI Cluster 32bits. Helm chart provided.

```bash
cd charts/kubeplay && helm install kubeplay . --values values.yaml --values values-arm32v7.yaml
```

### arm64v8

Deployment on KUBEDGE Raspberry PI Cluster 64bits. Helm chart provided.

```bash
cd charts/kubeplay && helm install kubeplay . --values values.yaml --values values-arm64v8.yaml
```

### amd64

Deployment on KUBEDGE CoreOS/Ubuntu Cluster. Helm chart provided.

```bash
cd charts/kubeplay && helm install kubeplay . --values values.yaml --values values-amd64.yaml
```
