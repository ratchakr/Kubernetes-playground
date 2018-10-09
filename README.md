# Kubernetes-playground
This is for exploring k8s and prepare for CKA exam

## Set Up Kubernetes cluster using kubeadm

### Steps

#### Initialize the k8s cluster with kubeadm and flannel default cidr networking on the master node

    sudo kubeadm init --pod-network-cidr=10.244.0.0/16
	
#### Install pod networking	(Using flannel networking)
    sudo kubectl apply -f https://raw.githubusercontent.com/coreos/flannel/master/Documentation/kube-flannel.yml

#### Join other nodes into the cluster created in step 1 and 2 above
    sudo kubeadm join 172.31.106.137:6443 --token wmo1yx.rglsyywo91ux9b0b --discovery-token-ca-cert-hash sha256:7b9daa9ff708ead67c6033c354e4ab253a10d441899b841d2b94ec309de70940
	
	