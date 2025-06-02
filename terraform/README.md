1. Provision AWS EKS Cluster using Terraform
   
Provision an AWS EKS cluster with VPC, IAM roles, and managed node groups using Terraform.
- Creates VPC with public & private subnets
- Deploys EKS cluster
- Sets up managed node groups with autoscaling
- Outputs kubeconfig for cluster access


Command:-
==============
terraform init
terraform plan
terraform apply

After applying, we can generate kubeconfig like this:

aws eks update-kubeconfig --region us-west-2 --name demo-eks-cluster
kubectl get nodes


****  Terraform Modules Used  *****
terraform-aws-modules/vpc/aws
terraform-aws-modules/eks/aws
