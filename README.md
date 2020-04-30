# Helm charts for CORD

This repo contains helm charts forked from [CORD](https://opencord.org/)
and subsidiary projects, to be used to deploy SEBA on ARM architectures.

Thes charts are published on: <https://iecedge.github.io/helm-charts/cord>

Please see <https://guide.opencord.org/charts/helm.html> for more complete
documentation on the Opencord usecases and components.

Please see <https://wiki.akraino.org/pages/viewpage.action?pageId=18481623>
for more information in Akraino IEC Platform.

## Changing charts

When you make changes to charts, please make sure of the following:

1. Make sure the chart passes a strict lint with `helm lint --strict
   <chartname>`.  The `scripts/helmlint.sh` will check all charts.

2. When you modify a chart, you must increase the version in `Chart.yaml`. You
   may also need to update other charts that depend on your chart.
