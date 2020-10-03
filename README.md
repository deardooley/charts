# Agave Helm Repository

[Kubernetes Helm](https://github.com/helm/helm) charts to deploy the [Agave Platform](https://agaveplatform.org/) and supporting services needed to deploy, scale, and manage the platform from day 1 to day N.

## TL;DR

```bash
$ helm repo add agave https://helm.agaveplatform.org/charts
$ helm search repo agave
$ helm install my-release agave/platform
```

## Important notice: Helm v2 EOL :warning:

[On November 13, 2020, Helm v2 support will formally end](https://github.com/helm/charts#status-of-the-project), Agave's charts are compliant with Helm version 3 and above. No support is planned for version 2.

## Before you begin

### Setup a Kubernetes Cluster

To set up Kubernetes on public cloud platforms or bare-metal servers refer to the Kubernetes [getting started guide](http://kubernetes.io/docs/getting-started-guides/).

### Install Helm

Helm is a tool for managing Kubernetes charts. Charts are packages of pre-configured Kubernetes resources.

To install Helm, refer to the [Helm install guide](https://github.com/helm/helm#install) and ensure that the `helm` binary is in the `PATH` of your shell.

### Add Repo

The following command allows you to download and install all the charts from this repository:

```bash
$ helm repo add agave https://helm.agaveplatform.org/charts
```

### Using Helm

Once you have added the Helm repo, you can deploy an Agave Helm Chart into a Kubernetes cluster.

Please refer to the [Quick Start guide](https://helm.sh/docs/intro/quickstart/) if you wish to get running in just a few commands, otherwise the [Using Helm Guide](https://helm.sh/docs/intro/using_helm/) provides detailed instructions on how to use the Helm client to manage packages on your Kubernetes cluster.

Useful Helm Client Commands:
* View available charts: `helm search repo`
* Install a chart: `helm install my-release agave/<package-name>`
* Upgrade your application: `helm upgrade`

# License

Copyright (c) 2020 Bitnami

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
