# kubernetes

#Docker multi-node installation


#MASTER NODE

  $git clone https://github.com/kubernetes/kube-deploy
 
  $cd kube-deploy/docker-multinode
 
  $./master.sh


#Download kubectl binary file

  wget https://storage.googleapis.com/kubernetes-release/release/v1.0.1/bin/linux/amd64/kubectl


#Set PATH

  export PATH=$PATH:${kubectl_path}


#Visit UI

  $ kubectl cluster-info
  
  dashboad url will be listed


#WORKING NODE

  $ git clone https://github.com/kubernetes/kube-deploy
  
  $ cd docker-multinode
  
  $ sudo su
  
  $ export MASTER_IP=${SOME_IP}
  
  $ ./worker.sh


Now you are ready to build your own service on kubernetes
