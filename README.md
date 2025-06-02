# DevOpsInterviewAssignment

2. Deploy an NGINX Application using a Kubernetes Manifest

This project contains Kubernetes manifests to deploy an NGINX web server using a Deployment and a Service(NodePort)

Yaml Contents
- `nginx-deployment.yaml`
- `nginx-service.yaml`

Apply the manifests
kubectl apply -f nginx-deployment.yaml
kubectl apply -f nginx-service.yaml

Verify the resources
kubectl get deployments
kubectl get pods
kubectl get services

Accessing the Application using NodePort
curl http://<NodeIP>:<NodePort>
