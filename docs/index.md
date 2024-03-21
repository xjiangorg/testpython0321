# Trusted Application Pipeline Software Template

This application, **testpython0321**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/xjiangorg/testpython0321 ](https://github.com/xjiangorg/testpython0321 ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/xjiangorg/testpython0321-gitops ](https://github.com/xjiangorg/testpython0321-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **testpython0321-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **testpython0321-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/xjiangorg/testpython0321-gitops ) in the components/testpython0321/overlays/prod directory |  
| **testpython0321-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/xjiangorg/testpython0321-gitops ) in the components/testpython0321/overlays/prod directory | 