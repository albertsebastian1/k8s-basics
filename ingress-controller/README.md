# k8s-basics
## Ingress Controller Deployment
#### **Committed this working copy for easy access to right file as older versions was throwing errors**



#### _Version with Error : app.kubernetes.io/version: 0.34.1_

* Error details
_**while reading PROXY protocol**, client: xx.xx.xx.xx, server: 0.0.0.0:80_
_2021/03/22 10:00:26 [error] 1764#1764: *34644 **broken header**: "GET /HTTP/1.1 Host: xx.xx.xx.xx_

* This is related to service annotation **service.beta.kubernetes.io/do-loadbalancer-enable-proxy-protocol: 'true'** 

#### _Current Version which is working : app.kubernetes.io/version: 0.44.0_

**Source**: _https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.44.0/deploy/static/provider/cloud/deploy.yaml_

**Ingress Controller Deployment Guide**: _https://kubernetes.github.io/ingress-nginx/deploy/_