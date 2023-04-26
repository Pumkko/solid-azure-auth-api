# WHAT DID I LEARN

## Auth

It's really easy to set it all up, when creating the project we can choose Microsoft.identity. After that all that is needed is to update the settings with the correct TenantId and clientId

HOWEVER It is important to note that generating the project direcly with Microsoft.Identity will update the app registration in azure with a couple of callbacks urls. When I did it it removed my existing callback url to my solidApp breaking it in the process. It seems like those generated URL can be safely removed

## Azure

It's really not that difficult to set it all up, with SolidStart we need to add a Web application (not an SPA) and then through "Expose an API" we can set the different scopes we want for our app, scopes that will be requested during the login (see the SolidStart client) and voila
