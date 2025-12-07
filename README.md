# Sources

- https://www.youtube.com/watch?v=2CCZ8fcLyGk&t=16s

# What problems is the GitOps approach solving?

GitOps solves key challenges in managing Kubernetes infrastructure and deployments by using Git as the single source of truth.  

If you don't know about GitOps, you probably deploy your K8s resources in one of 2 ways:
- by running `kubectl apply`, which happens only once
- by using a CI/CD pipeline that runs that same command with each code change

But overtime, people make changes to these resources, so we're not sure what the actual state of the cluster is.  
Plus, there's no easy way to know what's deployed in the cluster without inspecting the cluster itself.  

GitOps solves these issues by:
1. storing all resources within a Git repository, which provides a full history with easy access to look at what's deployed
2. having your resources continuously synced into the cluster so that there cannot be any "configuration drift"

# Flux vs Argo CD

These are the 2 main tools when it comes to GitOps.  
Both are CNCF-graduated projects (CNCF stands for Cloud Native Computing Foundation) and used widely by many companies.  



1/37
