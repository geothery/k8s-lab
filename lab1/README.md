## LAB 1

Check that you have kubectl command on your server  

With kubectl :   
- display the cluster status 
- get the nodes details (number, version)
- list the namespace
- list the ressources (po,svc,...) of the different namespace

Create the deployment with four replicas :  
```kubectl apply -f deployment.yaml```

Check that the deployment is UP

Deploy the service :  
``` kubectl apply -f service.yaml``` 

To do also :  
* Check the log of the pod
* Use ```kubectl exec``` with the good parameters to start a busybox pod and curl the service.
* Check the internal DNS
* Port forward to the pod
* Perform a rolling update
