# Goals

1. Create a Kubernetes Cluster in Microsoft’s Azure Kubernetes Service (AKS) for the project infrastructure.
2. Once the cluster is created we are going to run our NodeWeightTracker application on top of AKS. This means that we need to write all the configuration files that are needed for running our application in a Kubernetes Cluster.
3. Update or CI/CD process to deploy our already dockerized application into the Kubernetes cluster.
4. Install the Nginx ingress controller.
5. The NodeWeightTracker application must be accessible from the internet.
6. The NodeWeightTracker application must be exposed to the internet on port 80.
7. The NodeWeightTracker must have at least 3 instances to ensure high availability.
8. Use configmaps/secrets to store your application configurations.
9. Helm: Package the kubernetes manifests using helm and use it to deploy your application in your CI/CD pipeline.
10. Terraform: Manage your Azure resources using Infrastructure as Code.


<img width="814" alt="Screen Shot 2022-05-07 at 12 03 05" src="https://user-images.githubusercontent.com/93793111/167247370-c3467a9a-f8ca-44c4-b4ba-27d68a16f874.png">

<img width="1040" alt="Screen Shot 2022-05-07 at 12 00 43" src="https://user-images.githubusercontent.com/93793111/167247376-011bac4f-3cbb-4af5-823b-1b8a55d19769.png">

<img width="615" alt="Screen Shot 2022-05-07 at 12 01 05" src="https://user-images.githubusercontent.com/93793111/167247378-e0530b92-1594-42e1-9254-6961e99b2944.png">=

# Node.js Weight Tracker


![Demo](docs/build-weight-tracker-app-demo.gif)

This sample application demonstrates the following technologies.

* [hapi](https://hapi.dev) - a wonderful Node.js application framework
* [PostgreSQL](https://www.postgresql.org/) - a popular relational database
* [Postgres](https://github.com/porsager/postgres) - a new PostgreSQL client for Node.js
* [Vue.js](https://vuejs.org/) - a popular front-end library
* [Bulma](https://bulma.io/) - a great CSS framework based on Flexbox
* [EJS](https://ejs.co/) - a great template library for server-side HTML templates

**Requirements:**

* [Node.js](https://nodejs.org/) 14.x
* [PostgreSQL](https://www.postgresql.org/) (can be installed locally using Docker)
* [Free Okta developer account](https://developer.okta.com/) for account registration, login

## Install and Configuration

1. Clone or download source files
1. Run `npm install` to install dependencies
1. If you don't already have PostgreSQL, set up using Docker
1. Create a [free Okta developer account](https://developer.okta.com/) and add a web application for this app
1. Copy `.env.sample` to `.env` and change the `OKTA_*` values to your application
1. Initialize the PostgreSQL database by running `npm run initdb`
1. Run `npm run dev` to start Node.js

The associated blog post goes into more detail on how to set up PostgreSQL with Docker and how to configure your Okta account.
