
## Introduction

Keycloak provides an authentication layer for applications. 

This is a customized Keycloak Helm chart aimed at making it possible to automatically import and customize pre-exiting Keycloak Realms and Client with a configurable Root URL parameter. .

This chart bootstraps a [Keycloak](https://github.com/bitnami/containers/tree/main/bitnami/keycloak) deployment on a [Kubernetes](https://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.


## Usage and Instructions

This chart works like any other Helm Chart.

The end user is able to specity customized chart values in the custom-values.yaml file.

The Root URL parameter can be specified in the custom-values.yaml file. 

The custom realm JSON file shold be placed in the /files directory and named custom-realm.json since it serves as a data source to the configMap.

Example Usage: helm install my-keycloak --values ./Keycloak-Helm-Charts/custom-values.yaml ./Keycloak-Helm-Charts

