1. ```kubectl create namespace argocd```

2. ```kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml```

3. ```kubectl port-forward svc/argocd-server 8089:80```

4. ```kubectl get secret argocd-initial-admin-secret -n argocd -o yaml```

5. ```echo <password> | base64 --decode```

