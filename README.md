# service-mesh
OpenShift Service Mesh Demos

## Step 1 Installing required Operators
Installation of required operators is automated using an Ansible playbook. run the command below to install

```
ansible-playbook install/install-operators.yaml --extra-vars=username=kubeadmin --extra-vars=password={{replace}} --extra-vars=apiserver={{replace}}
```

## Step 2 Create ServiceMesh control plane
Creation of ServiceMesh control plane and servicemesh member role configuration automated using an Ansible playbook. Run the command below to install

```
ansible-playbook smcp/deploy-smcp.yaml --extra-vars=username=kubeadmin --extra-vars=password={replace} --extra-vars=apiserver={replace}
```
