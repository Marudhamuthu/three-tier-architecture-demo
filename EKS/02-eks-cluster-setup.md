# Install EKS

Please follow the prerequisites doc before this.

## Install using Fargate

```
eksctl create cluster --name demo-cluster-three-tier-1 --region us-east-1
```

## Delete the cluster

```
aws eks list-nodegroups --cluster-name demo-cluster-three-tier-1 --region ap-south-1
aws eks delete-nodegroup --cluster-name demo-cluster-three-tier-1 --nodegroup-name <nodegroup-name>
eksctl delete cluster --name demo-cluster-three-tier-1 --region us-east-1
```



