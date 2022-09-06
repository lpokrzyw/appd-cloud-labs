# appd-labs

## setting things up
Edit variables.tf

```
terraform init
terraform validate
terraform apply --auto-approve
kubectl config current-context
kubectl get namespace
kubectl -n kube-system get pods
```

## cleanup 

```
terraform destroy --auto-approve
To re-create the cluster, we just need to use the command:
terraform apply --auto-approve
```

### Delete the kubectl config

```
kubectl config view
kubectl config delete-cluster <cluster-name>
kubectl config delete-user <user-name>
kubectl config delete-context <context-name>
```
