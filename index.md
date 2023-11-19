---
layout: page
title: 
subtitle: A groovy collection of easy-peasy scripts and serverless ready templates for Google Cloud serverless computing!
sitemap:
  priority: 0.9
---

Creating a microservices project with Google cloud serverless can be quite a puzzle. Juggling all those instances(Cloud functions, Cloud run) together? It's no walk in the park! But fret not, there is a nifty solution to turn your pain into gain.

Introducing "**cloudboot**"! It's like a magic wand for your Google Cloud serverless operations, but in the form of a simple command-line tool. Think of it as your trusty sidekick for supercharging development and deployment.

## Key Features
- **Easy Deployment** With cloudboot, deploying your cloud functions is a breeze.
- **Effortless trigger setup** Define and configure triggers with ease, choosing from HTTP, Firestore, PubSub, or Storage bucket triggers. Let cloudboot automatically create trigger resources upon deployment
- **Serverless ready templates** For You. Access a variety of serverless ready templates to start your projects with a helping hand.
- **Project Management** Keep your faas/microservices projects organized and easy to handle.

<br/>
## Installation and Running Instructions.

### Samurai way: [Run the CLI with Docker](https://github.com/cloudboot/cli-docker/tree/main).

#### Linux, bash

In a Bash terminal, use the following command to build the Cloud Boot Docker image:
```shell
docker build -t "cloudboot:latest" - < <(curl -s "https://raw.githubusercontent.com/cloudboot/cli-docker/main/Dockerfile")
```

Then, run the configuration script:
```shell
sh <(curl -s "https://raw.githubusercontent.com/cloudboot/cli-docker/main/install.sh")
```

#### Windows, powershell(v7.x)
To build the Docker image in a PowerShell terminal(Run as administrator), run the following command:

```shell
(Invoke-WebRequest -Uri "https://raw.githubusercontent.com/cloudboot/cli-docker/main/Dockerfile" -Method Get -ContentType Text).Content | docker build -t "cloudboot:latest" -
```

Then, run the configuration script:
```shell
(Invoke-WebRequest -Uri "https://raw.githubusercontent.com/cloudboot/cli-docker/main/install.ps1" -Method Get -ContentType Text).Content | Invoke-Expression
```


### The Ronin: [Run the Pythonic CLI on your own](https://github.com/cloudboot/cli).

1. Install the Google Cloud CLI. Please refer the [official installation guide](https://cloud.google.com/sdk/docs/install).

2. Install the Python library,
```shell
pip install cloudboot
```

### Stay tuned for future updates.
CloudBoot is actively being developed, with plans to add more features and improvements in the future. Stay tuned for exciting updates that will further enhance your serverless development experience with GCP.

<br/>
##### Please note:

This product is not officially endorsed by Google.
You should use this product at your own risk.

##### Disclaimer:

Google is not responsible for any damages caused by the use of this product.
