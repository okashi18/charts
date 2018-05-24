# Kubetoy 1.3.0

A Kubernetes Toy Application

This a simple Node.js app to be used with IBM Cloud Private demos.  It helps explore kubernetes deployments and persistent volumes.

This version no longer requires access to the Internet to get the style sheets (Bootstrap).  They have been copied locally
so this app can run in air-gapped systems.

## Configuration

### Parameters

This Helm chart has only a few values that can be overriden using the --set parameter.  The replica count is the only interesting value that you might change.

` helm install --name my-toy --set replicaCount=3  `


