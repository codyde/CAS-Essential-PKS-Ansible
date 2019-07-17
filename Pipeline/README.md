# Pipeline Requirements

This pipeline deploys Essential PKS using Heptio Labs Wardroom playbooks in conjunction with CAS. There are a number of configurations that need to take place in order for functionality to occur. You can remove tasks out of the YAML file to take them out of processes if you wish.

## Endpoint Requirements

* Agent Endpoint (for SSH)
* Infoblox (optional - but you need a DNS reservation for the load balancer name)

The pipeline heavily leverages parameterized values within its configuration. Create parameters for the following items and replace them in the Code Stream YAML file

## Parameters

* Ansible Host
* Ansible Password
* Infoblox Username
* Infoblox Password
* Infoblox Host
* SSH Pass (machine workloads)

## Extra Requirements

* Slack Webhook - Currently the pipeline uses a notification at every task completion via webhook. A slack webhook is useful for this.
