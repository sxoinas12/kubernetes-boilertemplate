### K8s Setup for Express API & MongoDB

This repository contains all the required yaml files in order to create a K8s cluster for an express API pod that communicates
internally with a MongoDB pod.

### kubectl apply commands must be run in the below order

    kubectl apply -f mongo-secret.yaml
    kubectl apply -f mongo.yaml
    kubectl apply -f mongo-configmap.yaml
    kubectl apply -f mongo-express.yaml
