<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/BlindGarret/personal-db">
    <img src="images/logo.png" alt="Logo" width="300">
  </a>

  <p align="center">
    Helm Repository Values for Home DB
    <br />
    <a href="https://github.com/BlindGarret/personal-db/issues">Report Bug</a> |
    <a href="https://github.com/BlindGarret/personal-db/issues">Request Feature</a>
  </p>
</p>

### Built With

* [Kubernetes](https://kubernetes.io/)
* [Docker](https://www.docker.com/)
* [Helm](https://helm.sh/)
* [MySQL](https://www.mysql.com/)

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

Requires a functional K8s cluster with admin access.

### Installation

1. Create the namespace
   ```sh
   kubectl create namespace personal-db
   ```
2. Add Helm Repo
   ```sh
   helm repo add bitnami https://charts.bitnami.com/bitnami
   ```
2. Install the chart
   ```sh
   helm install personal-db bitnami/mysql -f values.yaml -n personal-db --set auth.rootPassword=<Pass>
   ```


<!-- CONTACT -->
## Contact

Project Link: [https://github.com/BlindGarret/personal-db](https://github.com/BlindGarret/personal-db)
