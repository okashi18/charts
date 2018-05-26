![KubeToy](https://ibm-icp-coc.github.io/charts/repo/stable/duck.png "KubeToy logo")
# Kubetoy 1.4.0

A Kubernetes Toy Application

This a simple Node.js app to be used with IBM Cloud Private demos.  It helps explore kubernetes deployments, config maps, secrets and optionally (persistent volumes)

See the GitHub [documentation](https://github.com/IBM-ICP-CoC/KubeToy) for examples of how to use this 
app.


## Configuration

### Parameters

The only parameter of interest is related to the use of shared storage.  KubeToy can be used to experiment 
with shared storage, however this feature is only useful if you have direct access to the persistent 
volume that will be bound to this app's claim.  For example if the PV was a NFS share, you would want to 
ssh into the NFS server host (or any client bound to that server) to explore the filesystem with 
standard OS commands.  So the default is to not include this functionality with the deployment.  If you 
do, however, then feel free to change the `storage.useSharedStorage` value to `true`.



