# kube-cluster
Ansible playbooks for building Kubernetes cluster given the existence of SSH keys.

Reference: https://www.digitalocean.com/community/tutorials/how-to-create-a-kubernetes-cluster-using-kubeadm-on-ubuntu-18-04

## dashboard
Guide: https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/
Token command: kubectl -n kubernetes-dashboard describe secret $(kubectl -n kubernetes-dashboard get secret | grep admin-user | awk '{print $1}')
UI link: http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/#/overview?namespace=_all
