# Kubernetes-playground
This is for exploring k8s and prepare for CKA exam

## Set Up Kubernetes cluster using kubeadm

### Steps

--- initialize the k8s cluster with kubeadm and flannel default cidr networking on the master node
    sudo kubeadm init --pod-network-cidr=10.244.0.0/16
	
	
   
