<!---
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# gaian_docker

## Overview

The Dockerfile in this folder can be used to build a Docker image running
the latest Atlas master branch in standalone mode. It does this by setting
up necessary dependencies, checking out the master branch of Atlas from
GitHub, and then building Atlas. By default, this image will start the Atlas
on port 21000.

## Usage


1. Ensure that you have a recent version of Docker installed from
   [docker.io](http://www.docker.io).
2. Set this folder as your working directory.
3. Type `docker build -t gaian_docker .` to build a Docker image called **gaian_docker**.
   
