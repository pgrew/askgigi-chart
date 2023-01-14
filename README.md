Readme: https://github.com/searxng/searxng-helm-chart/tree/main/searxng

##

helm install askgigi --generate-name -n askgigi --values askgigi/values.yaml
kubectl expose deployment -n askgigi askgigi-1672098266 --type=LoadBalancer --name=askgigi-lb --port=80 --target-port=8080
