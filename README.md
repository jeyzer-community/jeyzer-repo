# jeyzer-repo
The jeyzer-repo project is a facade - for build and dev run purposes - over the Jeyzer Community repositories.
It must contain the master branch of the Jeyzer base and demo repositories from the GitHub jeyzer-repo.

Prerequisites
------------------

**IMPORTANT** :
To setup this project, you must under the current jeyzer-repo directory :

- Clone the base repository : 
  git clone https://github.com/jeyzer-repo/base

- Clone the demo repository :
  git clone https://github.com/jeyzer-repo/demo



Usage
------------------

- The Jeyzer Web Analyzer will load the base and demo repositories from this directory in a developer environment, 
  assuming that the local_first is set in the base.xml.

- The Maven build will assemble the base repository into a jeyzer-profiles-base-${jeyzer version}.zip file.
  Zip file is generated in the jeyzer-dist/target/distribution directory.

- The Maven build will assemble the demo repository into a jeyzer-profiles-demo-${jeyzer version}.zip file.
  Zip file is generated in the jeyzer-dist/target/distribution directory.



Build instructions
------------------

Jeyzer Repo project can be built with Maven.

Under the current directory, execute :

> mvn clean package

The jeyzer-all project is responsible for calling the current project builds.

  
 License
-------

Copyright 2020-2023 Jeyzer.

Licensed under the [Mozilla Public License, Version 2.0](https://www.mozilla.org/media/MPL/2.0/index.815ca599c9df.txt)