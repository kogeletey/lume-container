# Lume SSG container image

Fork for archive original repository [GitHub - lumeland/docker: Docker image for Lume](https://github.com/lumeland/docker)

Updated  `Lume` Docker image(s):

- Alpine Linux: [ghcr.io/kogeletey/lume-container:alpine](https://github.com/kogeletey/lume-container/pkgs/container/lume-container) (default)
- CentOS: [ghcr.io/kogeletey/lume-container:centos](https://github.com/kogeletey/lume-container/pkgs/container/lume-container)
- Debian: [ghcr.io/kogeletey/lume-container:debian](https://github.com/kogeletey/lume-container/pkgs/container/lume-container)
- Ubuntu: [ghcr.io/kogeletey/lume-container:ubuntu](https://github.com/kogeletey/lume-container/pkgs/container/lume-container)

## Updating Images

There is a (convenient) shell script to update all `Dockerfile` manifests automatically using standard UN*X utilities.

Just execute: `./update.sh` in the project's root, and if there is a new release, `LUME_VERSION` will be updated to that
version accordingly. Commit the changes, create a Pull Request (that will verify images build successfully), and when
merged, another pipeline will take care of building the images (again) and publishing them to Docker Hub.
