[![Apache Sling](https://sling.apache.org/res/logos/sling.png)](https://sling.apache.org)

&#32;[![Build Status](https://ci-builds.apache.org/job/Sling/job/modules/job/sling-org-apache-sling-resource-editor/job/master/badge/icon)](https://ci-builds.apache.org/job/Sling/job/modules/job/sling-org-apache-sling-resource-editor/job/master/)&#32;[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=apache_sling-org-apache-sling-resource-editor&metric=coverage)](https://sonarcloud.io/dashboard?id=apache_sling-org-apache-sling-resource-editor)&#32;[![Sonarcloud Status](https://sonarcloud.io/api/project_badges/measure?project=apache_sling-org-apache-sling-resource-editor&metric=alert_status)](https://sonarcloud.io/dashboard?id=apache_sling-org-apache-sling-resource-editor)&#32;[![Contrib](https://sling.apache.org/badges/status-contrib.svg)](https://github.com/apache/sling-aggregator/blob/master/docs/status/contrib.md) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

# Apache Sling Resource Editor

This module is part of the [Apache Sling](https://sling.apache.org) project.

The Apache Sling Resource Editor allows to edit Apache Sling content based on the Sling API. 

++ Installation ++
o First install the JSNodeTypes library here: 'contrib/commons/js/nodetypes'. You find the short installation instruction in its README file.
o Then use 'mvn install -P autoInstallBundle' to install this bundle to your local Sling instance at port 8080. 
o After that you find the web application at "/reseditor/.html" on your server.

++ Development with the Sling Resource Editor ++
o Use `mvn install sling:install` to deploy changes of Java classes
o To have frontend changes automatically deployed call `mvn install -P autoInstallBundle -Dsling.mountByFS=true`
o To run the build on your local machine call './grunt desktop_build' within the frontend directory. It includes tests with firefox and chrome.
o To have the less sources automatically compiled on change call `./grunt watch:less` in the frontend directory. Press Ctrl-Z to stop watching.
o To have the 'desktop_build' target triggered on changes in the frontend tests, less sources, JavaScript files and JSP sources use `./grunt watch:all` in the frontend directory and also press Ctrl-Z to stop watching.
o If you don't use 'localhost' as server and '8080' as port you can specify your values by using the environment variables 'SLING_SERVER' 'SLING_PORT'.

Enjoy!
