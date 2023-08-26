# This is an commit done by Ahmed Mokhtar
# argocd

### Making argocd manage itself
```bash
# First deploy argocd with the provided kustomization
kustomize build . | k apply -f -

# Now create an argocd application that will point to that kustomization so that any change in the files gets reflected
k apply -f argocd-app.yaml
```
