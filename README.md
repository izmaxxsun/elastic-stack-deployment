# elastic-stack-deployment
Installing Elasticsearch, Kibana, Fleet Server and APM without orchestration. The other ways to deploy are using Elastic Cloud (managed service), or ECE/ECK which provide orchestration for easier install, upgrades, and maintenance.

## Create Virtual Machine
Created on Azure with Windows Server 2022 Datacenter Azure Edition
Size
Standard E2s v3
vCPUs
2
RAM
16 GiB

## Gameplan
Following along with [Installing the Elastic Stack](https://www.elastic.co/guide/en/elastic-stack/current/installing-elastic-stack.html), we need to install the stack in order and we'll focus on the minimum needed here:
* Elasticsearch
* Kibana
* APM

## Installing Elasticsearch
1 - Following the [Windows install instructions](https://www.elastic.co/guide/en/elasticsearch/reference/8.4/zip-windows.html), download the .zip file.

2 - Run Elasticsearch from the command line

3 - Check it is running
curl --cacert http_ca.crt https://elastic:IVMTu3b5RF+-E3F7kOxY@localhost:9200 --ssl-no-revoke

## Installing Kibana

