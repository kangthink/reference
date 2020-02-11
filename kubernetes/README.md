# Kubernetes

```
# 빠른 실행을 위해 설정
$ alias k='kubectl'
```

다양한 오브젝트를 살펴보고, 생성, 수정, 삭제를 하고 싶을 때

오브젝트 목록
- node
- pod
- replicaset
- deployment
- service
- loadbalancer
- ingress
- volume
- configmap
- secret
- namespace



## 관찰

### get
```
# pod, replicaset, deployment, service 조회
kubectl get all

# node 조회
kubectl get no
kubectl get node
kubectl get nodes

# pod 조회
kubectl get po
kubectl get pod


# 결과 포멧 변경
kubectl get nodes -o wide
kubectl get nodes -o yaml
kubectl get nodes -o json
kubectl get nodes -o json |
      jq ".items[] | {name:.metadata.name} + .status.capacity"
```

### describe
```
# kubectl describe type/name
# kubectl describe type name
kubectl describe node <node name>
kubectl describe node/<node name>
```

### log
```
kubectl logs NAME
kubectl logs -f NAME
```
## 생성
```
kubectl apply -f FILENAME
```

## 삭제
```
kubectl delete NAME
kubectl deldete -f FILENAME
```
