# HCMUS-Intro_DevOps-gitops-spring-petclinic-microservices
Source of Truth for Source repo: https://github.com/DipHuy/HCMUS-Intro_DevOps-spring-petclinic-microservices
# Folder Structure
## argocd
Applications for Argo CD apply using following commands:

- dev.yaml
```
kubectl apply -f https://raw.githubusercontent.com/DipHuy/HCMUS-Intro_DevOps-gitops-spring-petclinic-microservices/refs/heads/main/argocd/dev.yaml
```
- staging.yaml
```
kubectl apply -f https://raw.githubusercontent.com/DipHuy/HCMUS-Intro_DevOps-gitops-spring-petclinic-microservices/refs/heads/main/argocd/staging.yaml
```

## Helm
Jenkins will change these values file to update status of dev and staging namespace.
- values-dev.yaml: dev namespace, update when Source repo main branch update
- values-staging: staging, update when Source repo release a new tag
