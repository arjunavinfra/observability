# observability

Pre Configuration requirment:

1.Install kind kubernetes in local machine https://kind.sigs.k8s.io/docs/user/quick-start/

2.Install MetalLB for exposing the traffic https://github.com/arjunavinfra/kubernetes/tree/master/networking/metalLB

3.Setup the CSVSERVER  project from https://github.com/arjunavinfra/csvserver

Steps

1. Install the promethus and alertmanager using kustamization

  ```kubectl apply -k ./ --force-conflicts=true --server-side```
  
  ```kubectl get all -n monitoring```
  
  ```kubectl get service/prometheus-svc -n monitoring```
  
  
  Goto the external IP address got from above comment

![image](https://user-images.githubusercontent.com/118735091/204282982-6e47d41e-421e-4950-b18d-e97271aa2b31.png)

![image](https://user-images.githubusercontent.com/118735091/204308426-c75a3f19-19d3-4c65-a881-5e4a06b23e14.png)
