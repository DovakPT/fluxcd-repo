# fluxcd-repo
fluxcd CDRs information


## GitRepository
Use this when you want to keep your Kubernetes cluster in sync with a Git repository. 
It fetches the contents of the repository at regular intervals and creates an artifact. 
This is useful for declarative configuration management and GitOps workflows.


## HelmRelease 
This is used to manage Helm charts in your Kubernetes cluster. 
It ensures that the Helm charts are installed, upgraded, or rolled back as defined in the Helm repository. 
It's ideal for managing application deployments and lifecycle using Helm.


## HelmRepository 
This CRD is used to fetch Helm chart metadata from a Helm repository. 
It periodically checks the repository for updates and creates an artifact with the Helm chart index. 
This is useful for keeping Helm charts up-to-date in your cluster.


## Kustomization 
Use this when you want to manage Kubernetes manifests using Kustomize. 
It allows you to apply overlays and patches to your Kubernetes manifests stored in a Git repository or S3 bucket. 
This is great for managing different environments (e.g., staging, production) with the same base configuration.


## OciRepository
This is used to manage OCI (Open Container Initiative) images. 
It fetches the image metadata and ensures that the images are available in your Kubernetes cluster. 
This is useful for managing container images and ensuring they are up-to-date.