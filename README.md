<h1 align="center">SDDI CKAN for Kubernetes</h1>

<p align="center">
    <em>an application stack for <a title="SDDI CKAN" href="https://github.com/tum-gis/SDDI-CKAN-Docker">SDDI CKAN</a> in a Kubernetes cluster</em>
    <br />
    <br />
    <a href="https://github.com/tum-gis/sddi-ckan-k8s/issues">Report Bug</a>
    ·
    <a href="https://github.com/tum-gis/sddi-ckan-k8s/issues">Request Feature</a>
    <br />
    <br />
    <a href="https://github.com/tum-gis/sddi-ckan-k8s/releases" title="Latest release">
    <img src="https://img.shields.io/github/v/release/tum-gis/sddi-ckan-k8s?sort=semver">
  </a>
</p>

**Warning**:
> This repository is an early stage of development. Use it at your own risk!

## :inbox_tray: Components

## :rocket: Usage

1. Get a fully-qualified domain name (FQDN) and configure it to point to the public IP address of
   the LoadBalancer service of your Nginx ingress controller.

2. Add and update Helm repo

   ```console
   helm repo add sddi-ckan https://tum-gis.github.io/sddi-ckan-k8s
   helm repo update
   ```


4. Install stack

   ```console
   helm install ckan sddi-ckan/sddi-ckan \
     -n ckan --create-namespace \
     --atomic --wait \
     --values my-values.yml
   ```

## :construction_worker: Building

## :hammer_and_wrench: Contributing

Bug fixes, issue reports and contributions are greatly appreciated.

### Contributors

* This repo is based on the CKAN [Docker images](https://github.com/keitaroinc/docker-ckan)
  and [Helm charts](https://github.com/keitaroinc/ckan-helm) of
  [Keitaro](https://github.com/keitaroinc). Many thank's for your great work!

<a href="https://github.com/tum-gis/sddi-ckan-k8s/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=tum-gis/sddi-ckan-k8s" />
</a>

## :mortar_board: Research

## :memo: License

This Helm chart is distributed under the Apache License 2.0. See [LICENSE](LICENSE) for more information.

## :handshake: Thanks
