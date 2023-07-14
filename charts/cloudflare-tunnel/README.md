[![version](https://img.shields.io/badge/version-1.0.1-green.svg)](https://semver.org) ![ci](https://github.com/conventional-changelog/standard-version/workflows/ci/badge.svg)
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
|tunnel.token.create|bool|`true`|Create a secret for the tunnel from `token.value`|
|tunnel.token.value|str|-|The tunnel token string provided by cloudflare|
|tunnel.tokenSecretRef.name|str|`none`|The name of an existing tunnel token secret|
|tunnel.tokenSecretRef.key|str|`none`|The key to look for in the tunnel token secret|
