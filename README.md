# Book Shelf API - Helm Chart

This Helm chart deploys the following services:

- API app (`api-app`)
- PostgreSQL (`postgres`)

## Install

```bash
git clone https://github.com/kostaskara21/book-shelf-api-java-charts.git
cd book-shelf-api-java-charts
helm install my-book-shelf .
```

## Check Deployment

```bash
kubectl get pods
kubectl get svc
```

## Access API Locally

```bash
kubectl port-forward svc/api-service 8080:8080
```

Make call with  Postman:

```
http://localhost:8080
```

## Upgrade Chart

```bash
helm upgrade my-book-shelf .
```
