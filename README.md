# QpidJMS

The QpidJMS project provides a JMS based client that uses the AMQP v1.0 protocol.

Below are some quick pointers you might find useful.

## Building the code

The project requires Maven 3. Some example commands follow.

Clean previous builds output and install all modules to local repository without
running the tests:

    mvn clean install -DskipTests

Install all modules to the local repository after running all the tests:

    mvn clean install

Perform a subset tests on the packaged release artifacts without
installing:

    mvn clean verify -Dtest=TestNamePattern*

Execute the tests and produce code coverage report:

    mvn clean test jacoco:report

## Examples

First build and install all the modules as detailed above (if running against
a source checkout/release, rather than against released binaries) and then
consult the README in the qpid-jms-examples module itself.

## Documentation

There is some basic documentation in the qpid-jms-docs module.

## Distribution assembly

After building the modules, a distribution assembly can be found at:

    qpid-jms-assemblies/apache-qpid-jms/target
