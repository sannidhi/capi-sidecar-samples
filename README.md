# capi-sidecar-samples

Sample apps demonstrating how to use [sidecar processes](http://v3-apidocs.cloudfoundry.org/version/release-candidate/#sidecars) in Cloud Foundry.

## Apps
This repository currently contains the following sample apps and sidecars.

You can quickly deploy both apps by targeting your Cloud Foundry api using the `cf cli` and running the `push_sample_app_with_sidecar.sh` script.

### config-server-sidecar
A simple Golang binary that emulates a "configuration server" for the parent app to call out to.

### sidecar-dependent-app
A simple Sinatra app that calls out to the `config-server-sidecar` binary and echoes back its response.
