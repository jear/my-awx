# my-awx
https://docs.ansible.com/projects/awx-operator/en/latest/installation/basic-install.html

```
kubectl create ns awx
helm repo add awx-operator https://ansible-community.github.io/awx-operator-helm/
helm install awx-operator awx-operator/awx-operator -n awx

```
