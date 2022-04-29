使用官网[yaml](https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml)

然后修改name为argocd-server的Service中的type为LoadBalancer(L9753)


```bash
kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo
```
