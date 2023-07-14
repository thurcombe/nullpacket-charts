# nullpacket-charts

[![](https://github.com/thurcombe/nullpacket-charts/workflows/Release%20Charts/badge.svg?branch=main)](https://github.com/thurcombe/nullpacket-charts/actions)

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up properly, add the repo as follows:

```console
helm repo add nullpacket https://thurcombe.github.io/nullpacket-charts/
```

You can then run `helm search repo nullpacket` to see the charts.

## Charts

* [cloudflare-tunnel](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/cloudflare-tunnel) ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22cloudflare-tunnel%22%5D%5B0%5D.version&label=latest%20release)
