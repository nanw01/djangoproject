kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.5.0/aio/deploy/recommended.yaml

k describe secret -n kube-system

kubectl proxy

Kubectl will make Dashboard available at http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/.

```bash
brew tap weaveworks/tap

brew install weaveworks/tap/eksctl

eksctl version

eksctl create cluster \
--name test-cluster \
--version 1.17 \
--region us-east-1 \
--nodegroup-name linux-nodes \
--node-type t2.micro
--node 2


```