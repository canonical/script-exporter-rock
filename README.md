# script-exporter-rock

[![Publish to GHCR:dev](https://github.com/canonical/script-exporter-rock/actions/workflows/rock-release-dev.yaml/badge.svg)](https://github.com/canonical/script-exporter-rock/actions/workflows/rock-release-dev.yaml)
[![Update ROCK](https://github.com/canonical/script-exporter-rock/actions/workflows/rock-update.yaml/badge.svg)](https://github.com/canonical/script-exporter-rock/actions/workflows/rock-update.yaml)

[ROCKs](https://canonical-rockcraft.readthedocs-hosted.com/en/latest/) for the Prometheus [Script Exporter](https://github.com/ricoberger/script_exporter).  
This repository holds all the necessary files to build ROCKs for the upstream versions we support. The Script Exporter ROCK is used by the [script-exporter-operator](https://github.com/canonical/script-exporter-operator) charm.

Automation takes care of:
* validating PRs, by simply trying to build the ROCK;
* pulling upstream releases, creating a PR with the necessary files to be manually reviewed;
* releasing to GHCR at [ghcr.io/canonical/script-exporter:dev](https://ghcr.io/canonical/script-exporter:dev), when merging to main, for development purposes.
