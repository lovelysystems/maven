======================================
Lovely Systems Public Maven Repository
======================================

This repository contains the following artifacts:

:ls-hive: see: https://github.com/lovelysystems/ls-hive
:elasticsearch-ls-plugins: see: https://github.com/lovelysystems/elasticsearch-ls-plugins
:lovely-db-testing: see: https://github.com/lovelysystems/lovely-db-testing


Configuration
=============

To add this repository to your standard Maven project, add the following lines
to your ``pom.xml`` or ``settings.xml`` file::

 <repositories>
   <repository>
     <id>ls-releases</id>
     <url>https://raw.github.com/lovelysystems/maven/master/releases</url>
  </repository>
  <repository>
    <id>ls-snapshots</id>
    <url>https://raw.github.com/lovelysystems/maven/master/snapshots</url>
  </repository>
 </repositories>


Releases
========

To create a new release in this repository clone it to a folder next to your project.

In your project:

* setup a maven repos using `url = uri("../maven/releases")`
  (see `example <https://github.com/lovelysystems/lovely-db-testing/blob/0.0.3/build.gradle.kts#L35-L47>`_)

* run `gradlew publish`

After that commit the files added by publishing the project
