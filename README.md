## Install

This chart is still in an experimental phase, and it has not yet been published.

## Development

1. Clone this repo
2. Install dependencies 
    2.1 [Helm](https://helm.sh/docs/intro/install/)
    2.2 [Minikube](https://minikube.sigs.k8s.io/docs/start/)
3. run `helm install ocis .`

Verifying everything is running smooth can be done with `kubectl get services` and `kubectl get pods`; be sure to check on the pod status for errors, especially after committing an upgrade. If you want to update anything, modify the chart's `values.yaml` and run `helm upgrade ocis .`

### Dry runs
There are time when before upgrading you'd like to see the output of the yaml files that will be sent to Kubernetes, for that there is a little helper script `dry-run.sh`.