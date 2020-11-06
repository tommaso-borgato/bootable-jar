# JAX-RS WildFly bootable jar example

Build a bootable JAR containing a JAX-RS resource.

Build and run locally
=============

* To build: `mvn package`
* To run: `mvn wildfly-jar:run`
* Access the application: `http://127.0.0.1:8080/hello`

Build and run in OpenShift
=============

* To build and run: `oc new-app registry.access.redhat.com/ubi8/openjdk-11~https://github.com/tommaso-borgato/bootable-jar`
* To expose: `oc expose svc/bootable-jar`