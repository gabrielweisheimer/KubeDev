## Comando para execução:
https://github.com/kubernetes/ingress-nginx/tree/main/charts/ingress-nginx

helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
helm repo update

helm install ingress-nginx ingress-nginx/ingress-nginx --version 4.4.2 -f values.yml -n ingress-nginx

