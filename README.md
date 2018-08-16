# kube-ambassador

example setup to create an Ingress-Controller with ambassador

## Deploy Ambassador + demo application 
``` 
kubectl apply -f ambassador.yaml
kubectl apply -f service.yaml
kubectl apply -f qotm.yaml

```

## Test the setup

get the LoadBalancer URL
``` 
kubectl get services -o wide
```


```` 
curl -v <LOADBALANCDER-URL>/qotm
````



