# infra-dev


## K8s blue green testing
```
$ kubectl create -f nginx_blue_deploy.yaml 
deployment.apps/nginx-blue created
```
```
$ kubectl create -f nginx_green_deploy.yaml 
deployment.apps/nginx-green created
```
```
$ kubectl create -f nginx_service.yaml 
service/nginx created
```
```
$ kubectl edit svc nginx
```
* when editing the service, change **track** bettwen `blue` and `green`
