# my-awx
https://docs.ansible.com/projects/awx-operator/en/latest/installation/basic-install.html

https://github.com/ansible/awx/blob/devel/INSTALL.md

```
kubectl create ns awx
#helm repo add awx-operator https://ansible-community.github.io/awx-operator-helm/
#helm install awx-operator awx-operator/awx-operator -n awx

# With Kustomize
kubectl apply -k .

kubectl get pods -l "app.kubernetes.io/managed-by=awx-operator"
kubectl get svc -l "app.kubernetes.io/managed-by=awx-operator"
 
kubectl patch svc awx-demo-service -n awx -p '{"spec": {"type": "LoadBalancer"}}'

```
