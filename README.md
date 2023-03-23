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

Values that are recommended to be overwritten : 
- namespace 
- appName
- deployment.author
- deployment.image (your app)
- ingress.annotations.cert-manager.io/cluster-issuer
- ingress.annotations.kubernetes.io/ingress.class: (default : nginx)


  
   