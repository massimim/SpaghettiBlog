---
layout: post
title: Nvidia nsys and Containers
subtitle: pdf version
tags: [profiling, docker, nvidia, linux, tools, sysadmin]
comments: false
---

Nsys is an essential tool profiling. To make it work into a docker container environment some steps need to be taken. Here what to do: [here](https://developer.nvidia.com/blog/nvidia-nsight-systems-containers-cloud/)



```bash
sudo sh -c 'echo kernel.perf_event_paranoid=2 > /etc/sysctl.d/local.conf'
```
or
```bash
sudo sh -c 'echo 2 >/proc/sys/kernel/perf_event_paranoid'
```





