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

## Listar clusters

```
k3d cluster list
```

## Deletar Cluster
```
k3d cluster delete <NomeDoNovoCluster>

```
## Criar cluster com múltiplos nós

```
k3d cluster create <NomeDoNovoCluster> --servers 2 --agents 3

```
## Listar nodes ativos

```
kubectl get nodes
```