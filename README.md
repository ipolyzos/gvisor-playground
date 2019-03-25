# Overview
   [gVisor](https://github.com/google/gvisor) is a user-space kernel, written in [Go](https://golang.org/), that implements a substantial portion of the Linux system surface. 
 
   It includes an [Open Container Initiative (OCI)](https://www.opencontainers.org) runtime called _runsc_  that provides an isolation boundary between the application and the host kernel while integrates also  with [Docker](https://www.docker.com/) and [Kubernetes](https://kubernetes.io/).

   This project aims to serve as a local playground to explore and furher experiment with current [gVisor](https://github.com/google/gvisor) version. 

# Prerequisites
 - Any Linux (amd64) distro.
 - [Direnv](https://direnv.net/)
 - [Docker](https://docker.com)

# Tools   

The tools that are downloaded during env initialisation are:

 - [curl](https://curl.haxx.se/)
 - [Kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/)
 - [Minikube](https://github.com/kubernetes/minikube)

# Usage / Initialise workspace

## Initialize the workspace
```
$ direnv allow 
```

Initialization will create the _${PWD}/bin/_ folder and will download any required binaries e.g _runsc_ , _minikube_ etc. 

Instructions on how to enable the _runsc_ on docker are to be printed as the result of this initialization phase.

# References

- [gvisor](https://github.com/google/gvisor)

# License

```
  Copyright 2019 Ioannis Polyzos

  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

  Unless required by applicable law or agreed to in writing, software
  distributed under the License is distributed on an "AS IS" BASIS,
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
```
