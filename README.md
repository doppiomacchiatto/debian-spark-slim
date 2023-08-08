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

Production loads - migrate docker compose to Kubernetes.
