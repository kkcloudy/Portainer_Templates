ARG ${base_version}=v1.29

#### Use tailscale/tailscale:v1.26.0 as the base
FROM tailscale/tailscale:${base_version} AS base

# Copy launch script that expose env vars for tailscaled args
COPY launch.sh .
