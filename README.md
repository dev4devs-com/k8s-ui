# k8s-ui

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Overview 

This project is a Helm Chart which will install the [Kubernetes Dashboard](https://github.com/kubernetes/dashboard). 

Dashboard is a web-based Kubernetes user interface. You can use Dashboard to deploy containerized applications to a Kubernetes cluster, troubleshoot your containerized application, and manage the cluster resources.

## Pre-requirements

- [Helm](https://helm.sh/docs/intro/install/) 

## Usage

Following the steps to let you know how to use it. 

1. Clone this project:

```sh
$ git clone git@github.com:dev4devs-com/k8s-ui.git
``` 

2. Install the chart with helm:

```sh
$ helm install kubernetes-dashboard ./k8s-ui
``` 

**NOTE**

If you are seen the `error: listen tcp 127.0.0.1:8001: bind: address already in use` when you run `kubectl proxy` to checkout it then just kill the process as follows and re-run the command to do the bind. 

```sh
 $ ps aux | grep proxy
 kill -9 <pid kubectl proxy>
```

## Documentation:

- This chart is following the steps in: https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/
- It will create the [roles permissions](https://kubernetes.io/docs/reference/access-authn-authz/rbac/) as described in: https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md


**NOTE** This project is a basic example done as an POC, however, please feel free to contribute with it. 
