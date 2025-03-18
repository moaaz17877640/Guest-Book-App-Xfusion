# Guest-Book-App-Xfusion

Welcome to the Guest Book App Kubernetes Setup! This project contains the necessary configurations and scripts to deploy the Guest Book App on a Kubernetes cluster.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Guest Book App is a simple application where users can leave comments or messages. This repository contains the Kubernetes deployment files to set up and run the Guest Book App on a Kubernetes cluster.

## Features

- Kubernetes deployment and service configurations.
- Horizontal Pod Autoscaling.
- ConfigMaps and Secrets management.
- Persistent Volume Claims for data storage.

## Prerequisites

Before you begin, ensure you have the following prerequisites:

- [Kubernetes](https://kubernetes.io/) cluster setup.
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/) command-line tool installed.
- [Helm](https://helm.sh/) package manager installed (if using Helm charts).

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/username/Guest-Book-App-Xfusion.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Guest-Book-App-Xfusion
   ```

## Usage

### Deploying the Application


2. Deploy the Guest Book App:
   ```sh
   cd /backend 
   kubectl apply -f  .
   cd ..
   cd /frontend
   kubctl apply -f .
   ```

3. Verify the deployment:
   ```sh
   kubectl get pods
   kubectl get services
   ```

### Accessing the Application

1. Get the external IP address of the service:
   ```sh
   kubectl get service <svc-name> -o wide
   ```

2. Open your browser and navigate to the external IP address to access the Guest Book App.

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```sh
   git checkout -b feature-branch
   ```
3. Make your changes and commit them:
   ```sh
   git commit -m "Description of your changes"
   ```
4. Push to the branch:
   ```sh
   git push origin feature-branch
   ```
5. Create a pull request.

## License

This project is licensed under the MIT License.
```

Feel free to customize this `README.md` file according to your project specifics
