# PV-and-PVC
Kubernetes Persistent Volume (PV) and Persistent Volume Claim (PVC) Setup

This repository contains YAML configurations and a simple script to create and apply a Kubernetes Persistent Volume (PV) and Persistent Volume Claim (PVC). The provided files enable users to easily set up persistent storage within a Kubernetes cluster.

Files Included:
create_pv_and_pvc.sh: A short script to create both a Persistent Volume (PV) and a Persistent Volume Claim (PVC) for 10GB of storage.
pv.yaml: YAML configuration to create a Persistent Volume (PV) of 10GB with a hostPath and a Persistent Volume Claim (PVC) for 10GB storage.
pvc.yaml: YAML configuration for only the Persistent Volume Claim (PVC) setup (in case you already have a PV available).
Instructions:
To create and apply both PV and PVC:
Run the create_pv_and_pvc.sh script to create both resources.
To apply PVC-only configuration:
Use pvc.yaml to create a PVC that will bind to an available Persistent Volume in your cluster.
Customization:
You can change the storage size, access modes, and storage class based on your specific requirements.
For the hostPath volume, ensure the specified directory (/mnt/data) exists on the Kubernetes node, or modify it to match your environment.
Prerequisites:
A running Kubernetes cluster.
kubectl installed and configured.
