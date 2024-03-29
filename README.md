[![CircleCI](https://circleci.com/gh/giantswarm/prometheus-pushgateway-app.svg?style=shield)](https://circleci.com/gh/giantswarm/prometheus-pushgateway-app)

# prometheus-pushgateway chart

Giant Swarm offers a prometheus-pushgateway App which can be installed in workload clusters.
Here we define the prometheus-pushgateway chart with its templates and default configuration.

## ⛔️DEPRECATED prometheus-pushgateway-app chart

This is repository is no longer actively maintained or updated.

Instead we recommed using the [upstream chart](https://github.com/prometheus-community/helm-charts/tree/main/charts/prometheus-pushgateway)

## Installing

There are several ways to install this app onto a workload cluster.

- [Using our web interface](https://docs.giantswarm.io/ui-api/web/app-platform/#installing-an-app).
- By creating an [App resource](https://docs.giantswarm.io/ui-api/management-api/crd/apps.application.giantswarm.io/) in the management cluster as explained in [Getting started with App Platform](https://docs.giantswarm.io/app-platform/getting-started/).

## Configuring

### values.yaml

**This is an example of a values file you could upload using our web interface.**

```yaml
# values.yaml

```

### Sample App CR and ConfigMap for the management cluster

If you have access to the Kubernetes API on the management cluster, you could create
the App CR and ConfigMap directly.

Here is an example that would install the app to
workload cluster `abc12`:

```yaml
# appCR.yaml

```

```yaml
# user-values-configmap.yaml

```

See our [full reference on how to configure apps](https://docs.giantswarm.io/app-platform/app-configuration/) for more details.

## Compatibility

This app has been tested to work with the following workload cluster release versions:

- _add release version_

## Limitations

Some apps have restrictions on how they can be deployed.
Not following these limitations will most likely result in a broken deployment.

- _add limitation_

## Credit

- https://github.com/prometheus-community/helm-charts/blob/main/charts/prometheus-pushgateway
