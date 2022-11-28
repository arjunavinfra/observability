# observability

Pre Configuration requirment:

1.Install kind kubernetes in local machine https://kind.sigs.k8s.io/docs/user/quick-start/

2.Install MetalLB for exposing the traffic https://kind.sigs.k8s.io/docs/user/loadbalancer/ 

3.Run the CSVSERVER  project from https://github.com/arjunavinfra/csvserver

Steps

1. Install the CRD first 

  ```cd prometheus-operator-crd```
  
  ```kubectl create -k ./```
  
2. Install the promethus and alertmanager using kustamization

  ```cd .. ```
  
  ```kubectl apply -k ./```
  
  ```kubectl get all -n monitoring```
  
  ```kubectl get service/prometheus-svc -n monitoring```
  
  
  Goto the external IP address 

![image](https://user-images.githubusercontent.com/118735091/204282982-6e47d41e-421e-4950-b18d-e97271aa2b31.png)
