# Kubernetes-playground
This is for exploring k8s and prepare for CKA exam

## Set Up Kubernetes cluster using kubeadm

### Steps

#### Initialize the k8s cluster with kubeadm and flannel default cidr networking on the master node \n

    sudo kubeadm init --pod-network-cidr=10.244.0.0/16
	
#### Install pod networking	(Using flannel networking)
    sudo kubectl apply -f https://raw.githubusercontent.com/coreos/flannel/master/Documentation/kube-flannel.yml

