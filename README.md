# Kubernetes Microservice Flask Application

This is a microservice application built using Flask and deployed on Kubernetes. It is designed to demonstrate how to build and deploy microservices on a Kubernetes cluster.

![k8s micro](https://github.com/prajwalpd7/microservices-k8s/assets/71492927/5b4ff721-5d22-43e9-9230-2b18ad2d6204)


- Deploy a scalable Flask application and MongoDB on a Kubernetes cluster.


## Installation

To install and run the application on your Kubernetes cluster, follow these steps:

1. Clone this repository to your local machine.
2. Navigate to the project root directory.
3. Create a Kubernetes deployment and service by running the following command:

`kubectl apply -f kubernetes.yaml`

4. Verify that the deployment and service have been created successfully by running the following command:

`kubectl get deployments,services`

5. If everything is working properly, you should see the name of your deployment and service listed in the output.

## Usage

To use the microservice, you can send HTTP requests to the service's endpoint. Here's an example request:

`curl http://<service-ip>:<service-port>/tasks`


This should return a JSON response with a greeting message.


## Project Roadmap

### Phase 1: Environment Setup
- Install Kubernetes and initialize a cluster using kubeadm.
- Set up `kubectl` for cluster management.

### Phase 2: Application Development
- Develop a Flask application serving as the microservice.
- Connect the application to MongoDB.

### Phase 3: Dockerization
- Create Dockerfiles for both Flask and MongoDB.
- Build and test Docker images locally.

### Phase 4: Kubernetes Deployment
- Create YAML files for deployments and services.
- Deploy the components to the Kubernetes cluster.

### Phase 5: Scalability
- Implement Horizontal Pod Autoscaling.

### Phase 6: Monitoring and Logging
- Set up Prometheus and Grafana for monitoring.
- Use Fluentd and Elasticsearch for logging.

### Phase 7: Troubleshooting
- Implement best practices for troubleshooting common issues.

