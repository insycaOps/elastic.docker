# ElasticSearch image for Azure Container Instance (ACI) deployment 
based on "Dockerfiles for the official Elastic Stack images". https://github.com/elastic/dockerfiles/tree/7.7

Azure Container Instances are limited in defining environment variables. For a quick deployment and customer showcase setup a single-node Elasticsearch instance is sufficient. Due to the limitation, we build a ready to use image.

## Azure Container Group Deployment (Elasticsearch and Kibana)

Microsoft Deployment Tutorial: https://docs.microsoft.com/en-us/azure/container-instances/container-instances-multi-container-yaml.

Follow the instructions from the tutorial and use modified "deploy-aci.yaml" for ready-to-use Elasticsearch and Kibana Container.

## Azure CLI Command for Deployment:
az container create --resource-group YOUR-RESOURCE-GROUP --file deploy-aci.yaml

deploy-aci.yaml file can be found here: https://github.com/insycaOps/elastic.docker/blob/master/deploy-aci.yaml

## Blogarticle with Step-by-Step Guide
https://insyca.home.blog/2020/06/02/elasticsearch-und-kibana-docker-images-fur-azure-container-instance-aci/
