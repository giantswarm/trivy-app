[![CircleCI](https://circleci.com/gh/giantswarm/trivy-app-app.svg?style=shield)](https://circleci.com/gh/giantswarm/trivy-app-app)

# trivy-app chart

Giant Swarm offers a trivy App which can be installed in workload clusters.
Here we define the trivy chart with its templates and default configuration.

**What is this app?**
**Why did we add it?**
**Who can use it?**

## Installing

There are 3 ways to install this app onto a workload cluster.

1. [Using our web interface](https://docs.giantswarm.io/ui-api/web/app-platform/#installing-an-app)
2. [Using our API](https://docs.giantswarm.io/api/#operation/createClusterAppV5)
3. Directly creating the [App custom resource](https://docs.giantswarm.io/ui-api/management-api/crd/apps.application.giantswarm.io/) on the management cluster.

## Configuring


### Sample App CR and ConfigMap for the management cluster


## Compatibility


## Limitations

## Development

### Subtrees

This repo is configured to have a `git subtree` split folder `helm/trivy` from `https://github.com/giantswarm/trivy-upstream` at `helm/trivy-app/charts/trivy/` in the local repository.

## Credit

* https://github.com/aquasecurity/trivy
