#### kubectl commands

kubectl get nodes\
kubectl get pod\
kubectl get services\
kubectl get deployment\
kubectl get replicaset

#### debugging

kubectl logs {pod-name}\
kubectl exec -it {pod-name} -- bin/bash


#### delete

kubectl delete deployment {deployment-name}\
kubectl delete service {service-name}

#### edit deployment

kubectl edit deployment {deployment-name}