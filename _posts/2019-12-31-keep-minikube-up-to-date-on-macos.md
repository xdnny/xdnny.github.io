---
layout: post
title: "Keep Minikube up to date on macOS"
date: 2020-10-27 03:20:11 +0100
categories: [DevOps]
tags: [kubernetes,python]
---

Two components are required in order to use [Kubernetes](https://kubernetes.io) in form of [Minikube](https://minikube.sigs.k8s.io/docs): `minikube` and `kubectl`.

Default approach might be to use [Homebrew](https://brew.sh) or [MacPorts](https://www.macports.org), however if you happen to prefer to skip package managers, here is a script which makes sure Minikube stack is always up to date.

[minikube-latest.py](https://gist.github.com/xdnny/5684efdf33dd451f364f5910102a182d)

The script is written in [Python](https://python.org), so Python modules [PyGithub](https://github.com/PyGithub/PyGithub) and [Requests: HTTP for Humans™](https://requests.readthedocs.io/en/master) need to be installed.

It works as an initial installation as well. If you have one of [supported virtualization platforms](https://minikube.sigs.k8s.io/docs/drivers/) available, you can start instantly by running `minikube start`.
