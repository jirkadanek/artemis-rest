# artemis-rest

[![Build Status](https://travis-ci.org/jdanekrh/artemis-rest.svg?branch=master)](https://travis-ci.org/jdanekrh/artemis-rest)

Standalone example of ActiveMQ Artemis REST API. See also https://github.com/apache/activemq-artemis/tree/master/examples/features/standard/rest and the documentation at 
https://github.com/apache/activemq-artemis/blob/master/docs/user-manual/en/rest.md (at the time of writing, the current REST documentation released with 1.3.0 contained errors)

Build a project with `mvn package` in the project directory and drop the `.war` file to a directory on an application server.

There are two projects in this repository.

## embedded

Artemis broker is embedded in the `.war` file and runs inside the application server (like Tomcat or Jetty).

## integrated

Artemis broker is integrated in the application server (like WIldfly 10). Broker in application server must be properly configured (e.g. create the queues you need). The `.war` won't work in application servers that do not integrate Artemis broker (Tomcat or Jetty).
