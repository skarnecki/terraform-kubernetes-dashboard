# terraform-kubernetes-dashboard

This module will configure and deploy Kubernetes dashboard to cluster configured in provider. 

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| app_name | Value of k8s-app label | string | `kubernetes-dashboard` | no |
| k8s_dashboard_ver | Version of Kubernetes dashboard to deploy | string | `1.10.1` | no |
| minimal_role_name | Name of limited permissions role | string | `kubernetes-dashboard-minimal` | no |
| name | Name of deployed service | string | `kubernetes-dashboard` | no |
| namespace | Target namespace to deploy | string | `kube-system` | no |
| replicas | Number of replicas | string | `1` | no |
| revision_history_limit | Revision history limit | string | `10` | no |