# k8s-ui

## Overview 

This project is a Helm Chart which will install the [Kubernetes Dashboard](https://github.com/kubernetes/dashboard). 

Dashboard is a web-based Kubernetes user interface. You can use Dashboard to deploy containerized applications to a Kubernetes cluster, troubleshoot your containerized application, and manage the cluster resources.

**NOTES**
- This chart follow the steps in: https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/
- It will create the [roles permissions](https://kubernetes.io/docs/reference/access-authn-authz/rbac/) as described in: https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md