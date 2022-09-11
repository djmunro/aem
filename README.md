# Creating Docker containers for Adobe Experience Manager

In this repository you will find the dockerfiles needed to create an Author, Publish and a Dispatcher.

## Building

### AEM base image

```
docker build -t aem .
```

All at once using the docker compose command or one by one

```
docker-compose up
```

### AEM Publish image

```
docker build -t publish .

docker run -p 4503:4503 publish
```

### AEM Author image

```
docker build -t author .

docker run -p 4502:4502 author
```

## Resources

- [Creating Docker containers for Adobe Experience Manager - Video](https://youtu.be/7vBrN53HkoQ)
- [Creating Docker containers for Adobe Experience Manager - Post](https://www.dlighthouse.co/2018/08/creating-docker-containers-aem.html)
- [Github link for the code](https://github.com/drginm/docker-boilerplates/tree/master/005-adobe-experience-manager)
- [What is AEM](https://helpx.adobe.com/experience-manager/6-3/sites/deploying/using/deploy.html#WhatisAEM)
- [Typical Deployment Scenarios](https://helpx.adobe.com/experience-manager/6-3/sites/deploying/using/deploy.html#TypicalDeploymentScenarios)
- [Installing the Dispatcher](https://helpx.adobe.com/experience-manager/dispatcher/using/dispatcher-install.html)
- [Downloading the Dispatcher](https://www.adobeaemcloud.com/content/companies/public/adobe/dispatcher/dispatcher.html)
- [Configure Run Modes](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/configure-runmodes.html)
- [Default Local Install](https://helpx.adobe.com/experience-manager/6-3/sites/deploying/using/deploy.html#DefaultLocalInstall)
- [AEM Technical Requirements](https://helpx.adobe.com/experience-manager/6-3/sites/deploying/using/technical-requirements.html)
- [Add Instruction - Dockerfile reference](https://docs.docker.com/engine/reference/builder/#add)
- [Create an AEM app using Adobe\'s archetype](https://helpx.adobe.com/experience-manager/using/maven_arch12.html#CreateanAEMMaven12archetypeproject)
