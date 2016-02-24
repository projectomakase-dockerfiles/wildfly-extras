# WildFly Extras Docker Image #

This repository contains the Dockerfile for creating a Wildfly instance with the Modeshape and Camel sub-systems.

### Image ###

The image **extends** the `projectomakase/wildfly:latest` image and adds Modeshape 4.5 and the Wildfly Camel Extension 3.3.0.

### Availability ###

The Dockerfile is available in the master branch and is built in the Docker HUB as projectomakase/wildfly-extras:latest.

### Usage ###

To boot in standalone mode

    docker run -d projectomakase/wildfly-extras

### Environment Variables ###

The image supports the following environment variables:

### `ADMIN_USER`

If provided will create a wildfly managerment user with the given user name, ADMIN_PASSWORD is also required for this to work. This is required to access the Wildfly and Hawt.io management console.

### `ADMIN_PASSWORD`

If provided will create a wildfly managerment user with the given password, ADMIN_USER is also required for this to work. This is required to access the Wildfly and Hawt.io management console.
