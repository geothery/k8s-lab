## LAB2 : Deploy a microservice application

Directory lab2 :

You will deploy a microservice application (php + redis) :  
  - Check the yaml file in descriptors directory
  - From the yaml file, draw the application architecture (nb of pods / services)
  - Deploy the application (in your namespace !!! )
  - Scale the number of frontend pod (up to 5) and check the pod status
  - Can you access the application ? What is it missing to access it from Internet ?

Add an Ingress : 

```
apiVersion: extensions/v1beta1
kind: Ingress
metadata:
  name: basic-ingress
spec:
  backend:
    serviceName: frontend
    servicePort: 8080
```
