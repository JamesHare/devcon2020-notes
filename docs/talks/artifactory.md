# Artifactory

What is Artifactory?

Artifactory is a binary repository manager responsible for managing finary artifacts.

* Internal dependencies
* External dependencies
* Storing built artifacts including container images
* Global distribution of artifacts

Package Types

Can handle many package types including:

* chef
* docker
* rubygems
* ivy
* maven
* rpm/yum

Things to know

* Artifactory implements a checksum-based storage
    * No duplication in physical storage
* Repository types
    * Local
    * Remote
    * Virtual - A combination of local and remote
* Replication types
    * push
        * events like create, copy, move and delete.
    * pull
        * used for remote repositories to pre-populate the cache
