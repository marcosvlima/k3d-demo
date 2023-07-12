# k3d-demo
K3D Demo lab

## Install K3d

```
wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
```

## Install kubectl

```
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
rm -rf kubectl
```

## Criar novo cluster

```
k3d cluster create <NomeDoNovoCluster>
```

## Apply Demo Wordpress

```
kubectl apply -f manifest.yaml
```