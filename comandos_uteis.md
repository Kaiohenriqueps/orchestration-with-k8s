# Comandos Úteis

## Criando um recurso (pod, replicaset, dpeloyment):
```
$ kubectl create -f arquivo.yaml
```
## Listando recursos: 
```
$ kubect get {pods,replicaset,deployment}
```
## Deletando recursos:
```
$ kubectl delete replicaset nome-do-replicaset
```
## Atualizando recurso:
```
$ kubectl replace -f arquivo.yaml
```
## Escalando recurso:
Obs: serve tanto para aumentar quando para diminuir
```
$ kubectl scale replicas=x -f arquivo.yaml
```
## Status do deployment:
```
$ kubectl rollout status deployment/nome-deployment
```
## Aplicando mudança no deployment:
Obs: irá atualizar o deployment de acordo com a mudança
```
$ kubectl apply -f deployments/dp.yaml
```
## Rollout para uma versão anterior:
```
$ kubectl rollout undo deployment/nome-deployment
```