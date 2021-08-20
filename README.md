GSoC submission 2021
===================

### GSoC-2021_EAT_JBoss-Community

----------

Introduction
-------------

EAT is a testsuite to develop tests against infinite number of JBoss servers. It’s an innovative tool because it’s creating the test once and testing with any version of the tested software.The idea behind the project, the AT (Additional Testsuite) structure, covers a wide variety of new features that could be added to it. One of them, is the addition of a CI (Continuous Integration) tool to perform some automated testing operations. EAT is available for a number of server configurations and a CI pipeline can be built using the maven tool.


#### Advantages of EAT:

1. Writing the tests once and testing against infinite number of Application Servers.
2. Having all the tests at one place.
3. Comparison of the servers based on the testsuite.
4. Guarding against regression.
5. Faster convergence among the servers.
6. Comparison of the servers based on tests of the past and the present.
7. Addition of tests with possible future features that are not at the moment available.
8. It makes possible to push a testcase of a fix regarding a specific component of the server, without the component version to have been updated at the server pom.


#### Project Description

The EAT (Eap Additional Testsuite) got extended by adding a new subcategory for testing the latest, at that time, JBoss Community server. The newly added subcategory was made available for use with the CI builds.

Support for the Gradle tool was built to integrate it with the EAT framework, allowing Gradle-based builds to take advantage of the EAT framework’s capabilities.



Project Timeline - Results
------------------------------

The implementation of this project was divided in two phases:

#### Phase 1

At the begining of the 1st phase of this project I studied the documented features of the new, at that time, JBoss versions. 

Afterwards, I downloaded and built the [Wildfly](https://github.com/wildfly/wildfly) JBoss server and then tested it using [EAT](https://github.com/EAT-JBCOMMUNITY/EAT).

The next step was to add the 24.0.0 version of the Wildfly server in EAT [EAT PR 1](https://github.com/EAT-JBCOMMUNITY/EAT/pull/159).

Finally, I studied the support for lifecycles offered by Maven and Gradle, in order to be able to implement basic support for integrating Gradle with the EAT during the next phase of the project.


#### Phase 2

During the 2nd phase of this project, I implemented basic support for integrating Gradle with the EAT framework and specifically the Wildfly Server [EAT PR 2](https://github.com/EAT-JBCOMMUNITY/EAT/pull/171).

List of Commits
----------------------------
[f1e0468](https://github.com/EAT-JBCOMMUNITY/EAT/commit/f1e0468834a7f067ad06a5f2fc57d8853bee439b) Adding Wildfly 24.0.0
[3b9dbd3](https://github.com/EAT-JBCOMMUNITY/EAT/commit/3b9dbd39f02fea6a47c70e5b3f5fe462641454de) Adding Gradle Support for the Wildfly Server

PROJECT URL
----------------------------
[Project URL](https://github.com/EAT-JBCOMMUNITY/EAT)

EAT WORKSHOP
----------------------------
[EAT Workshop](https://www.dropbox.com/s/bebhyd1iz7cg1i2/EAT_WORKSHOP.odt?dl=0)
