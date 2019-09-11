---
layout: post
title: "Build une image Docker dans un conteneur Docker"
description: "Docker in docker"
category: 
tags: [Docker]
---

C'est facile, il suffit de monter le volume du binaire et de la socket dans le conteneur qui sera en charge de builder une image docker.

```   
docker run -it 
    -v /usr/bin/docker:/usr/bin/docker 
    -v /var/run/docker.sock:/var/run/docker.sock  
    imageName uild/tfs-agent-dotnetcore /bin/bash

```   