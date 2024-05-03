1. get list of persistent volume sorted by capacity
```
kubectl get pv -o yaml
kubectl get pv --sort-by .spec.capacity.storage > /home/cloud_user/pv_list.txt
```
2. execute command inside quark's container to find the key value of /etc/key/key.txt file
`kubectl exec quark -c busybox -n beebox-mobile -- cat /home/cloud_user/key.txt`

