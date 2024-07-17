## kubernetes

### Services and Networking
#### List pods in wide format, display IP Address 
```
$ kubectl run nginx --image=nginx --port=80
pod/nginx created
$ kubectl get pod nginx -o wide
```

#### Get CIDR of a node
```
kubectl get nodes minikube -o json | jq .spec.podCIDR
```

#### USing busybox, curl pod using its IP address
```
kubectl run busybox --image=busybox --rm -it --restart=Never -- wget 172.17.0.4:80
```


