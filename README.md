# API-peliculas-teis

Para crear las imagenes y desplegarlas puede utilizar los siguientes comandos:
```
docker build -t imagen .
docker tag imagen usuarioDocker/imagen
docker push usuarioDocker/imagen
```

Para dezplegar la base de datos y la API utilice los siguientes comandos:

BD:
```
kubectl create -f db-deployment.yaml
kubectl create -f db-service.yaml
```
API:
```
kubectl create -f api-deployment.yaml
kubectl create -f api-service.yaml
```
Para verificar que todo este en orden y la API y DB ya se encuentren desplegadas puede utilizar los siguientes comandos:
```
kubectl get services
kubectl get deployments
kubectl get pods
```
