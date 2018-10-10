# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM ubuntu:16.04

RUN apt-get update && apt-get -y upgrade && apt-get install -y openjdk-8-jdk git python unzip
ENV JAVA_HOME /usr/lib/jvm/java-8-openjdk-amd64

ENV PATH /usr/lib/jvm/java-8-openjdk-amd64/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin

# Working directory
WORKDIR /root/gaian

ADD dist/GAIANDB_V2.1.8_20160523.zip /root/gaian
RUN unzip GAIANDB_V2.1.8_20160523.zip

# Working directory
WORKDIR /root/gaian

ENV PATH /root/atlas-bin/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin

EXPOSE 6414

CMD ["/bin/bash", "-c", "/root/gaian/launchGaianServer.sh"]
#CMD ["/bin/bash", "-c", "sleep 10000000"]
