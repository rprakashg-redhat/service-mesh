# service-mesh
OpenShift Service Mesh Demos

## Step 1 Installing required Operators
Installation of required operators is automated using an Ansible playbook. Follow steps below to install the required operators on OpenShift cluster

```
ansible-playbook install/install-operators.yaml --extra-vars=username=kubeadmin --extra-vars=password={{replace}} --extra-vars=apiserver={{replace}}
```

## Step 2 Create ServiceMesh control plane