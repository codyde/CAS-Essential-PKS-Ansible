# Notes on these Ansible plays

The playbooks within this directory are used to prepare the NGINX server for deployment, acting as a load balancer for the k8s master nodes.

The deployment of the Kubernetes workloads is handled through [Wardroom](https://github.com/heptiolabs/wardroom). I am using a special fork of this project located [here](https://github.com/codyde/wardroom) - to upgrade the deployment to Kubernetes 1.15.

## Required Structure

Process

* Navigate to your playbooks directory
* Clone this Repository
* CD to that directory
* Clone the [Wardroom fork](https://github.com/codyde/wardroom)
