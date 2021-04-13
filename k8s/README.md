# Desafio 3

## Para Rodar o Aplicativo
### Primeiro instale o kind depois rode:
```
$ kind create cluster --config=kind.yml
$ kubectl cluster-info --context kind-imersao-fsfc2

$ kubectl apply -f backend/
$ kubectl apply -f frontend/

$ kubectl port-forward service/backend-service 3000
$ kubectl port-forward service/frontend-service 80

#run on http://localhost:80
```