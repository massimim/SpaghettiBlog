---
layout: post
title: nvidia container runtime
subtitle: pdf version
tags: [nvidia, cuda, docker, container, linux, tools, sysadmin]
comments: false
---

Interesting post on how to use docker containers on ubuntu and nvidia GPUs: [here](https://towardsdatascience.com/how-to-properly-use-the-gpu-within-a-docker-container-4c699c78c6d1).

The key takeaway is an ubuntu package called `nvidia-container-runtime`

```bash
apt-get install nvidia-container-runtime
docker run -it --rm --gpus all ubuntu nvidia-smi
```



