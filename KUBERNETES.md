## kubernetes

### Services and Networking
#### List pods in wide format, display IP Address 
```
$ kubectl run nginx --image=nginx --port=80
pod/nginx created
$ kubectl get pod nginx -o wide
```
