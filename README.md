# ArgoCD-EFK-Deploy

## Intro

All the necessary yaml files to deploy the elsticsearch, fluentd and kibana in kubernetes

## Folder structure

The folder structure is as follows :

```bash

      --- environments
      |     |
      |     --- overlays
      |           |
      |           --- prod
      |                 |
      |                 --- namespace
      |                 |     |
      |                 |     --- limit-range.yaml
      |                 |     --- namespace.yaml
      |                 |     --- resource-quota.yaml
      |                 --- shared
      |                 |     |
      |                 |     --- shared-resousrce (i.e pv)
      |                 |
      |                 --- kustermization.yaml
      |
      --- manifests
            |
            --- services
                  |
                  --- elasticsearch-fluentd-kibana
                        |
                        --- base
                              |
                              --- elasticsearch-service.yaml
                                  elasticsearch-statefulset.yaml
                                  fluentd-configmap.yaml
                                  fluentd-daemonset.yaml
                                  kibana-deploy.yaml
                                  kibana-service.yaml
                                  kustomization.yaml

```
            

