FROM mcr.microsoft.com/devcontainers/rust:1-1-bullseye

# Install dependencies in one layer and clean up
RUN apt-get update && \
  DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
  libwebkit2gtk-4.0-dev \
  build-essential \
  curl \
  wget \
  file \
  libssl-dev \
  libgtk-3-dev \
  libayatana-appindicator3-dev \
  librsvg2-dev && \
  apt-get clean && \
  rm -rf /var/lib/apt/lists/*