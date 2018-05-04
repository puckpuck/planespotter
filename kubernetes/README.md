## Installing on Kubernetes

1. Run `kubectl create namespace planespotter`
1. Optionally create a kubectl config context pointing to the new namespace [kubectl set-context docs](https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#-em-set-context-em)
1. Install app: `kubectl apply -f .`
1. Get bash shell on MySQL pod (pod name may be different) `kubectl exec -it mysql-0 bash`
1. Configure database [database install](./db-install)

## Getting URL from within minikube

1. Run `minikube service -n planespotter planespotter-frontend --url`
