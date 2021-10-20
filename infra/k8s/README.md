# MicroServiceWithNodeJsReactJs

# Guide (https://kubernetes.github.io/ingress-nginx/deploy/#provider-specific-steps)

# below is complusry cmd to runt ingress Nginx
kubectl wait --namespace ingress-nginx --for=condition=ready pod --selector=app.kubernetes.io/component=controller --timeout=120s

# Note to run ingress Nginx for kurbernetes 
# The mandatory.yaml has been replaced. Follow this procedure:

# 1. install krew, the package manager for kubectl, see https://krew.sigs.k8s.io/docs/user-guide/setup/install/
# 2. install ingress-nginx by typing into a command prompt: kubectl krew install ingress-nginx.
# 3. then rerun the specific command: kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.40.1/deploy/static/provider/cloud/deploy.yaml
# All this assumes that (Docker and) Kubernetes is running.
#Happy orchestrating!