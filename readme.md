## create cm  
`kubectl create configmap km-config --from-file=config.toml=kube-monkey-config.toml`  

## logs  
`kubectl logs -f $(kubectl get pods | tr ' ' '\n' | grep kube-monkey)`
