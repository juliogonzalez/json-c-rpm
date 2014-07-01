json-c
======

CentOS/RH/Amazon RPMs for json-c <https://github.com/json-c/json-c>

Based off the RPM package created by Jussi Lehtola and upgraded by [Fedora Release Engineering](https://fedoraproject.org/wiki/ReleaseEngineering)

Tested on x64 CentOS 6.4 and Amazon Linux 2014.03


Requirements
------------

* pkgconfig
* libtool
* GCC, GCC-C++
* rpm-build


Building fresh RPMs
-------------------

Clone the repo: 

    git@github.com:juliogonzalez/json-c-rpm.git
    cd json-c-rpm

Optional: You can choose a version to be built by using git tags.

To get the version list:

    git tag

To checkout to a particular version:

    git checkout <tag>

Build the json-c RPMs
---------------------

Build the RPMs:

    ./json-c-rpm

And install:

    rpm -Uvh RPMS/$HOSTTYPE/json-c-0.10-1.*.$HOSTTYPE.rpm

You may use the following command:

    ./clean

To clean up the build environment (this will delete RPMs as well)
