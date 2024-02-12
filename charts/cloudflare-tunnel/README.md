![Dynamic YAML Badge](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fthurcombe%2Fnullpacket-charts%2Fgh-pages%2Findex.yaml&query=%24.entries%5B%22cloudflare-tunnel%22%5D%5B0%5D.version&label=latest%20release&link=https%3A%2F%2Fgithub.com%2Fthurcombe%2Fnullpacket-charts%2Freleases)

# cloudflare-tunnel

This helm chart install cloudflared in tunnel mode. 

**Homepage:** https://github.com/thurcombe/nullpacket-charts/tree/main/charts/cloudflare-tunnel

## Installation

First ensure that you've setup [cloudflare zero trust](https://one.dash.cloudflare.com/). 

Create a tunnel in Access/Tunnels. Using the provided token, either pre-create the kubernetes secret
and set `tunnel.token.create` to `false`, then configure `tunnel.tokenSecretRef` accordingly. 
Alternatively, the chart will create a secret for the token if `tunnel.token.create` is true and 
you provided the token in `tunnel.token.value`

Using [Helm](https://helm.sh), you can easily install and test cloudflare in a Kubernetes cluster by running the following:

```bash
helm repo add nullpacket https://thurcombe.github.io/nullpacket-charts/
```

#### Install Chart

Now install the chart:
```bash
helm upgrade --install \
  my-release \
  nullpacket/cloudflare-tunnel \
  -f values.yaml
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
|image.repository|str|cloudflare/cloudflared|The cloudflared image to use|
|image.tag|str|chart app version|The image tag to deploy|
|image.pullPolicy|strIfNotPresent|The image pull policy to use|
|tunnel.token.create|bool|`true`|Create a secret for the tunnel from `token.value`|
|tunnel.token.value|str|-|The tunnel token string provided by cloudflare|
|tunnel.tokenSecretRef.name|str|`none`|The name of an existing tunnel token secret|
|tunnel.tokenSecretRef.key|str|`none`|The key to look for in the tunnel token secret|
|tunnel.protocol|str|quic|The tunnel protocol to use|
|metrics.enabled|bool|false|Denotes if metric service should be enabled|
|metrics.port|integer|60123|The port number the metrics server should listen on|
|metrics.bind_address|str|0.0.0.0|The IP address to bind the metrics server to|
|metrics.prometheus_label.key|str|release|The key for the prometheus label required for scraping|
|metrics.prometheus_label.value|str|promstack|The value for the prometheus label required for scraping|



