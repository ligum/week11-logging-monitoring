# MONITORING AND LOGGING

![image](https://bootcamp.rhinops.io/images/monitoring-logging.gif)

## OVERVIEW

Monitoring provides feedback from production and delivers information about an application’s performance and usage patterns. When performance or other issues arise, relevant data about the issues are sent back to development teams through automated monitoring. Besides helping us track issues that may arise in production we can also use monitoring to automatically scale up or down a specific service depending on it’s usage.

Monitoring covers different types of data but the most common are: metrics and logs. With metrics we can see how is the performance of our application and even the machines themselves, and with logs we can see exactly what is going on at the application level by inspecting the application logs.

We will focus on what happens after we deploy our applications to our environments. We are going to set up a monitoring system that consists on the Prometheus Stack to collect metrics and visualize them and the Elasticsearch Stack to collect logs and visualize them.

![image](https://bootcamp.rhinops.io/images/prom-elk.png)

## PROJECT
### Introduction
Up until now we wrote CI/CD pipelines for the NodeWeightTracker application. Once it gets deployed to the environments we want to be able to monitor all of our services so we need to collect metrics and logs. To be able to collect them and visualize them we are going to set up a Monitoring system. We will deploy together both the Prometheus and the Elasticsearch stacks into our Kubernetes cluster to understand how we can use them to improve our observability.

### Project Overview
Two workshops will be held this week:

Prometheus Stack: In this workshop we will see how to monitor a Kubernetes cluster infrastructure using the Prometheus Operator.

Elasticsearch Stack (ELK): In this workshop we will learn how to use the Elasticsearch operator to deploy a logging system in Kubernetes.

### Goals

Complete the Prometheus Workshop:

https://github.com/sela-rhinops/bootcamp-monitoring

Complete the Elasticsearch Workshop:

https://github.com/sela-rhinops/bootcamp-logging

### Considerations

Knowing monitoring tools is essential for any DevOps engineer. During this week we will study the most common Stacks but there are other similar tools that are used for the same purposes (Splunk, Datadog, etc)

In addition, each cloud provider offer their own solutions:

AWS: CloudWatch

GCP: Cloud Monitoring

Azure: Azure Monitor

### Expected Result

A monitoring system based on the Prometheus Stack is configured in your cluster

A logging system based on the ELK Stack is configured in your cluster

### Bonus

Redirect your WeightTracker application logs to store them into elasticsearch

Redirect your Ingress Controller logs to store them into elasticsearch in it’s own index

