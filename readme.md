# Tutorial

[VSCode Django Tutorial](https://code.visualstudio.com/docs/python/tutorial-django)

# Deploy Web-App to Azure

[Push to Azure Container Registry](https://code.visualstudio.com/docs/containers/tutorial-django-push-to-registry)

[Deploy to Azure Web Apps ](https://docs.microsoft.com/de-de/azure/developer/python/tutorial-deploy-containers-01)


## Notes

- Error: The subscription is not registered to use namespace 'Microsoft.Web'. See https://aka.ms/rps-not-found for how to register subscriptions.
    - Subscription muss über "Azure Portal -> Abonnements -> Ressourcenanbieter" registriert werden (im obigen Fall 'Microsoft.Web' registrieren)

- [After change: Redeploy](https://docs.microsoft.com/en-us/azure/developer/python/tutorial-deploy-containers-03)
    1. Re-Build Docker image (VSCode command line: 'Docker Images: Build Image...')
    2. Push image to registry (VSCode command line: 'Docker Images: Push...')
    3. Restart Azure App Service (VSCode Azure App Service Extension -> Right-Click Wep-App)