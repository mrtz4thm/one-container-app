# Basic one container application 
---
tested with helm version : 3.11.2 

## Prerequisites 

Kubernetes Cluster with :  
- Ingrescontroller (like nginx)
- ClusterIssuer 
- CertManager
- required secrets

Values that have to be overwritten : 
- domain 
- ingress.annotations.cert-manager.io/cluster-issuer (cluster issuer name)

Values that are recommended to be overwritten : 
- namespace 
- appName
- deployment.author
- deployment.image (your app)
- ingress.annotations.kubernetes.io/ingress.class: (default : nginx)


  
   