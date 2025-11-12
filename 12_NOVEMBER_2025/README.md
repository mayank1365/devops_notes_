# Docker Images

## Overview

Docker images are immutable templates that define how containers are built. Images are composed of layers which improve build performance and storage efficiency.

## Key Points

- `docker images` - List images
- `docker pull` - Download images
- `docker rmi` - Remove images
- `docker tag` - Manage image versions
- `docker history` - Inspect image layers
- **Layer Caching**: Speeds up image builds
- **Base Images**: Choose minimal images like alpine
- **Security**: Smaller images reduce attack surface
