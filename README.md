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

### Example function
```
def handler(event, context):
    print(event)
    return {'Hello': 'World'}
```

### `Deploy functions`
```
kubeless function deploy hello --runtime python3.6 --handler hello.handler --from-file hello.py
```

### `Call a function`
```
kubeless function call hello  --data  'aa'
```

### `Update a function`
```
kubeless function update hello --runtime python3.6 --handler hello.handler --from-file hello.py
```
