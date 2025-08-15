# Umami Fork

This is a forked repository of [umami-software/umami](https://github.com/umami-software/umami) with automated builds using Chalk and continuous integration workflows.

## Automated Workflows

This repository includes several automated workflows:

- **Sync Upstream**: Automatically syncs with the upstream repository every 30 minutes
- **Chalk and Push**: Builds Docker images with Chalk instrumentation and pushes to ECR
- **Weekly Production Build**: Retags dev images as production images every Wednesday

## Repository Structure

- `master` branch: Contains only this README and the workflow files
- `upstream` branch: Mirror of the upstream repository with latest changes
- Builds are triggered automatically when upstream changes are detected

## Chalk Integration

All Docker images are built with [Chalk](https://crashoverride.com/chalk) for enhanced security and observability.
