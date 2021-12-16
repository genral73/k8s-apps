### For production run it as deployments on k8s
```shell
git clone https://github.com/genral73/k8s-apps.git 

kubectl  apply -k  k8s-apps/sealedsecret-issuer
```
- Visit ingress host of deployment, in this case go to [https://sealedsecret-issuer.localhost/](https://sealedsecret-issuer.localhost/).



### For demo run it as container on localhost
```shell
docker run  -d  -p 8080:8080/tcp  genral73/sealedsecret-issuer:latest
```
- Go to [http://localhost:8080/](http://localhost:8080/).