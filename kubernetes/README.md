## Minikube
If you don't have a Kubernetes environment, minikube is a really easy way to get going.  To install it on your mac [go here](https://gist.github.com/kevin-smets/b91a34cea662d0c523968472a81788f7). Once installed you can follow the steps below to install this app.  If you alreayd have a Kubernetes environement, just install this app there.

## Wavefront Monitoring
Before installing you should have deployed Wavefront monitoring of your Kubernetes environment. You can use this sample [wavefront.yaml](wavefront/wavefront.yaml) as a template, be sure to replace the `CUSTOMER_CLUSTER` and `CUSTOMER_TOKEN` values accordingly.

## Installing Planespotter

1. Run `kubectl create namespace planespotter`
1. Install app: `kubectl apply -f .`

## Getting URL from minikube

1. Run `minikube service -n planespotter planespotter-frontend --url`
