# Inconsistent Build Environment in Dockerfile

This repository demonstrates a common issue in Dockerfiles: using outdated base images and unspecified Python versions. This can lead to inconsistent builds across different environments and unexpected runtime behavior.

## Problem

The original `Dockerfile` uses `ubuntu:latest`, which might not be the same across different Docker setups. Additionally, it does not explicitly define the Python version, relying on the default version present in the base image. This lack of specificity can lead to unpredictable results and breaks in the build process across machines and times.