# show_me_the_code_3_Aug

## Installing Local k8s [Minikube](https://github.com/kubernetes/minikube),  `kubectl` and `kubeless`

### Prerequisite
- `brew`
- `VirtualBox`

### Installation
- `brew cask install minikube`
- `brew install kubernetes-cli`
- [kubeless](https://github.com/kubeless/kubeless/releases)

### Start 
```
minikube start
```

### kubectl
```
kubectl get pods
```

## `Getting started`

### `Listing functions`

```
kubeless function list
```
