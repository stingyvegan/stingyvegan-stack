# StingyVegan Stack

Documentation, docker-compose and helm charts for the full stingyvegan suite of services

## Helm

Helm charts are provided to run the entire stingyvegan application easily in kubernetes.

```sh
# Add repository
helm repo add stingyvegan-helm https://helm.stingyvegan.com.au
# Install application into the `stingyvegan` namespace using chart
helm install -n stingyvegan stingyvegan stingyvegan-app
# Uninstall
helm uninstall -n stingyvegan stingyvegan
```

## Local Development

### Test helm chart locally

```sh
# Install using local chart
helm install -n stingyvegan stingyvegan ./helm
# Uninstall
helm uninstall -n stingyvegan stingyvegan
```
