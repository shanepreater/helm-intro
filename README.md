Helm examples
==============

This repo contains a couple of examples of helm charts for use with the Argo DevOps Helm introduction presentation.

Contents
------------

 * nginx - A very simple independant helm chart which installs a fully working nginx instance along with a default index,html.
 * example - An example of a helm chart which uses a dependent chart to create a bigger deployment foot print


Commands to try
----------------

During the demo the following commands were used:

 * `helm list` - This lists all the currently deployed helm charts in this environment.
 * `helm lint nginx` - This performs static checking of the nginx chart.
 * `helm install nginx nginx --dry-run` - This performs a dry run install of the nginx chart to show what resources are generated.
 * `helm install nginx nginx` - This performs the actual installation.
 * `helm upgrade nginx nginx` - This illustrates that charts can be upgraded once they are deployed.
 * `helm uninstall nginx` - This removes all deployed artifacts associated with the chart.
 * `helm dependency list` - This deploys the dependencies used by a chart (must be done in the same directory as the Chart.yaml).
 * `helm dependency build` - This popluates the charts directory with the dependant charts (must be done in the same directory as the Chart.yaml).

