# Automatic Deployment of a Hadoop-Spark Cluster using Terraform
---

This is a project I created for the `Big Data Systems & Techniques` course of my MSc in Data Science.
It's a very basic implementation of an orchestration systems that provisions and configures a 3-node cluster (the number of data-nodes can be easily extended) with Apache Hadoop and Apache Spark.

## Project's Task

The task of this project is to use the [Terraform](https://terraform.io) IAC (Infrastructure as Code) tool to automatically provision Amazon VMs and install Hadoop on the cluster.
The resources used are:
- Linux image: `Ubuntu 16.04`
- Java: `jdk1.8.0_131`
- Apache Hadoop: `hadoop-2.7.2`
- Apache Spark: `spark-2.1.1`

## What is Infrastructure As Code and what is Terraform?

Infrastructure as code is a new DevOps philosophy where the application infrastructure is no longer created by hand but programmatically. The benefits are numerous
including but not limited to:
- Speed of deployment
- Version Control of Infrastructure
- Engineer agnostic infrastructure (no single point of failure/no single person to bug)
- Better lifetime management (automatic scale up/down, healing)
- Cross-provider deployment with minimal changes

Terraform is a tool that helps in this direction. It is an open source tool developed by [Hashicorp](https://www.hashicorp.com/).

This tool allows you to write the final state that you wish your infrastructure to have and terraform applies those changes for you.

You can provision VMs, create subnets, assign security groups and pretty much perform any action that any cloud provider allows.

Terraform support a wide range of [providers](https://www.terraform.io/docs/providers/index.html) including the big 3 ones AWS, GCP, Microsoft Azure.
