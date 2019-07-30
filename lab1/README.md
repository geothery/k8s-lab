## LAB 1

Log in the kubernetes cluster :  
Create the deployment with four replicas :  
```kubectl apply -f deployment.yaml```

Check that the deployment is UP

Deploy the service :  
``` kubectl apply -f service.yaml``` 

To do also :  
* Check the log of the pod
* Use ```kubectl exec``` with the good parameters to start a busybox pod and curl the service.
