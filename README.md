## Tekton Setup
Tekton installation and pipeline setup


### Installation
Assuming you already have a running Kubernetes cluster and other components needed, the next thing to do is to apply the `Tekton` components' manifest. Note that the manifest to be applied are all latest version.

```bash
# Pipeline
kubectl apply --filename https://storage.googleapis.com/tekton-releases/pipeline/latest/release.yaml

# Triggers & Interceptors
kubectl apply --filename https://storage.googleapis.com/tekton-releases/triggers/latest/release.yaml
kubectl apply --filename https://storage.googleapis.com/tekton-releases/triggers/latest/interceptors.yaml

# Dashboard
kubectl apply --filename https://storage.googleapis.com/tekton-releases/dashboard/latest/release.yaml

```  

### Setup Pipeline & Triggers
```bash
# Apply all the manifest/files
kubectl apply --filename ./manifest

```  