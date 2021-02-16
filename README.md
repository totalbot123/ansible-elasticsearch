# ansible-elasticsearch

This is a project for installing Elasticsearch cluster

## Getting Started

Note that there isn't much to this project, as Elasticsearch is maintaining their ansible role, making setup of Elasticsearch an ease.

### Prerequisites

Ansible is required to run ansible playbook.

Downloading Elasticsearch role from ansible-galaxy is required:
```
ansible-galaxy install elastic.elasticsearch,v7.10.2
```

### Deployment

To deploy the cluster, you run:
```
ansible-playbook -i hosts init_es_cluster.yml
```

Where hosts is a hosts file. You'll notice that default host groups are "master" and "data" groups.
One other thing that you should change in playbook is "elasticmaster" host. Change it to hostname or IP address of the master.
