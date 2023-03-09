# Provisioning Compute Resources

Kubernetes requires a set of machines to host the Kubernetes control plane and the worker nodes where containers are ultimately run. In this lab you will provision the compute resources required for running a secure and highly available Kubernetes cluster across a single [compute zone](https://cloud.google.com/compute/docs/regions-zones/regions-zones).

> Ensure a default compute zone and region have been set as described in the [Prerequisites](01-prerequisites.md#set-a-default-compute-region-and-zone) lab.


## VMS 
Create the 6 VMs (anywhere) and onboard them on the tailscale network

The VM host name should be as the list bellow

### Verification

List the compute instances:

```
NAME
controller-0
controller-1
controller-2
worker-0    
worker-1    
worker-2    
```

## Configuring SSH Access

see: https://tailscale.com/tailscale-ssh/

Next: [Provisioning a CA and Generating TLS Certificates](04-certificate-authority.md)
