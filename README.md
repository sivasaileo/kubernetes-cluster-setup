
1. Create 2 instances on AWS or Azure or GCP enviroment for master and worker nodes

Next on master node, execute the below script.

### Setup master node

Execute the below commands on master node

Commands:

```
wget https://raw.githubusercontent.com/khajaehtesham/kubernetes-cluster-setup/refs/heads/main/cluster-setup/latest/install_master.sh
chmod +x install_master.sh
bash install_master.sh
```

### Setup worker nodes

On all of the worker nodes, execute the below script. 

Commands:

```
wget https://raw.githubusercontent.com/khajaehtesham/kubernetes-cluster-setup/refs/heads/main/cluster-setup/latest/install_worker.sh
chmod +x install_worker.sh
bash install_worker.sh
```
Open the required ports in the firewall (NSG)  - 30000-40000

Once this is done, your cluster would be ready, ensure your all nodes are showing as ready. Use below command to verify

```
kubectl get nodes 
```

