# Deployment Strategy

> In this document, I describe deployment strategy used for this whole GitHub organization and the reasons that motivated theses choices.
> To be efficient the deployment process 
> * must be simple enough so that deploying a new application take at most 10 mn.
> * must be entirely stateless so that everything can be deployed from scratch automatically.
> * must rely on continuous deployment so that application is always up to date

## Releases tagging

We are going to follow semantic versionning.

## Continuous delivery

![continuous-delivery-pipeline](../docs/images/continuous-delivery-pipeline.png)

## Continuous deployment

![continuous-deployment-pipeline](../docs/images/continuous-deployment-pipeline.png)