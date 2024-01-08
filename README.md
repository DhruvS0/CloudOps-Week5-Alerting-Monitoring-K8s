# CloudOps-Week5-Alerting-Monitoring-K8s

## Architecture
![Alt text](ezgif.com-gif-maker.gif)

**Image Credits-** [MallikarjunG](https://devo.hashnode.dev/comprehensive-aws-eks-cluster-monitoring-with-prometheus-grafanaand-efk-stack-10weeksofcloudops)
## Monitoring AWS EKS Cluster with Prometheus, Grafana, and ELK Stack

This guide walks you through setting up comprehensive monitoring for an AWS EKS cluster using Prometheus, Grafana, and the ELK stack. You'll deploy a sample chatbot application on EKS and configure the monitoring tools to collect metrics, visualize data, and analyze logs.

### Prerequisites:

- AWS account with IAM permissions to create EKS clusters and other resources.
- Basic understanding of Kubernetes and containerization

### Steps:

#### Step 1 - [Set Up the EKS Cluster](jounral/Step1.md)

Create an EKS cluster using the eksctl tool or the AWS console.
Configure cluster roles and service accounts for Prometheus and the ELK stack.

Deploy the Chatbot Application:

#### Step 2 - [Build and package the chatbot application as a Docker image](journal/Step2.md)
Deploy the application to the EKS cluster using a Kubernetes deployment manifest.

Configure Prometheus:

#### Step 3 - [Deploy the Prometheus and Grafana operator and scrape metrics from the EKS cluster and chatbot pods](journal/Step3.md)
Create Prometheus scrape configurations for the target pods and nodes.

Configure Grafana:

#### Step 4 - [Configure a datasource for Prometheus and Grafana](journal/Step4.md)
Create dashboards in Grafana to visualize key metrics from the chatbot application and EKS cluster.

Configure the ELK Stack:

#### Step 5 - [Deploy the ELK stack using the official Helm chart or Docker images](journal/Step5.md)
Configure Fluentd to collect logs from the EKS cluster and chatbot pods.
Configure Elasticsearch to store and index the collected logs.
Set up Kibana to visualize and analyze the logs.

Access the Monitoring Tools:

The Prometheus UI is available at `http://<prometheus_endpoint>:9090`.

The Grafana UI is available at `http://<grafana_endpoint>:3000`.

The Kibana UI is available at `http://<kibana_endpoint>:5601`.

Additional Notes:

This guide provides a basic setup for monitoring an EKS cluster. You can customize the monitoring configuration to meet your specific needs.
Consider using managed services like Amazon Managed Grafana or Amazon Elasticsearch Service for a more hands-off monitoring experience.

I hope this helps! Feel free to modify and expand this draft to fit your specific needs and project.