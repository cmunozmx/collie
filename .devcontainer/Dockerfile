FROM mcr.microsoft.com/devcontainers/rust:1-1-bullseye

# Install dependencies in one layer and clean up
RUN apt-get update && \
  DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
  libgtk-3-dev libwebkit2gtk-4.0-dev libappindicator3-dev librsvg2-dev patchelf