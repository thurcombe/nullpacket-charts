# nullpacket-charts

[![Release Charts](https://github.com/thurcombe/nullpacket-charts/actions/workflows/main.yml/badge.svg)](https://github.com/thurcombe/nullpacket-charts/actions/workflows/main.yml)

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up properly, add the repo as follows:

```console
helm repo add nullpacket https://thurcombe.github.io/nullpacket-charts/
```

You can then run `helm search repo nullpacket` to see the charts.

## Charts

| Chart | Description | Latest Version | Status |
|-------|-------------|----------------|--------|
|[cloudflare-tunnel](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/cloudflare-tunnel)| Deploy a cloudflared tunnel| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22cloudflare-tunnel%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity%20-deprecated%20-red)
|[jackett](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/jackett) | Deploy jackett| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22jackett%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|
|[jellyfin](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/jellyfin) | Deploy jellyfin| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22jellyfin%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|
|[qbittorrent](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/qbittorrent) | Deploy qbittorrent| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22qbittorrent%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|
|[sonarr](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/sonarr) | Deploy sonarr| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22sonarr%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|
|[prowlarr](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/prowlarr) | Deploy prowlarr| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22prowlarr%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|
|[sabnzbd](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/sabnzbd) | Deploy SABnzbd| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22prowlarr%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|
|[radarr](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/radarr) | Deploy radarr| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22radarr%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|
|[jellyseer](https://github.com/thurcombe/nullpacket-charts/tree/master/charts/jellyseer) | Deploy jellyseer| ![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22jellyseer%22%5D%5B0%5D.version&label=latest%20release)|![](https://img.shields.io/badge/maturity-alpha-orange)|

