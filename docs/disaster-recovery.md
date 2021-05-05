# Disaster recovery procedure

*In case of corruption of whole Cluster, spontaneous fire, meteorite crash... We need to be able to restore everything up and running in a few minutes*

## Re-deploy micro-services

> TODO: develop a script to iterate over existing repositories, check if `continuous-deployment.yml` workflow exists, and if so trigger it using *workflow_dispatch* event.
> It will require that `continuous-deployment.yml` to be able to deploy from latest version if no tag is provided...

**we need to update deployment process**

- build and publish docker
- (after success) bumpversion for master branch
- (after success [or workflow_dispatch]) continuous deployment from master branch

... not that easy to bumpversion automatically. Probably this is not feasible without a config file to normalize definition of current version.

## Micro-services' databases backups ?
