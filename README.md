# Debian Spark #
This project provides a docker file to build a Spark cluster on debian... The openjdk containers are going to be deprecated soon.  Thus, the need for this project.

The docker file is for Scala/Java and Spark.  In order to keep the distro light, we are not installing python and all the supporting packages for Apache Spark.

# Software Versions #
* Debian Bookworm-Slim
* Apache Spark 3.4.1 and Hadoop 3
* Java - Eclipse-temurin:11
* Scala 2.11.12
* SBT 1.9.x

# Master & Workers #
Use this image to start the Spark Master and the worker nodes with Docker Compose. (Development only)

```shell
sudo docker start -e SPARK_WORKLOAD=master spark-debian
```
Production loads - migrate docker compose to Kubernetes.


### License ###
*Copyright 2023 doppiomacchiato*

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
