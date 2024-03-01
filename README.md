## ArgoCD Applications per EKS Cluster

Name of the folder represent name of the EKS Cluster (Except HelmCharts).

```
│
├── HelmCharts             # All Helm Charts
│   ├── ChartTest1
│   │   ├── Chart.yaml
│   │   ├── templates
│   │   ├── values_dev.yaml    # DEV Values
│   │   └── values.yaml        # Default Values
│   └── ChartTest2
│       ├── Chart.yaml
│       ├── templates
│       ├── values_dev.yaml    # DEV Values
│       └── values.yaml        # Default Values
│   
├── demo-dev                   # EKS Cluster name
    ├── applications
    │   ├── app1.yaml
        └── root.yaml              # Root ArgoCD Application
```

This repository serves as an endpoint for Argo CD to search for updates to the Helm charts. It automatically detects and applies these changes, providing users with previews of how the updated charts will appear."
