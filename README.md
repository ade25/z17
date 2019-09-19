# Webserver z17

![Website](https://img.shields.io/website?down_message=offline&label=host%20z17&up_message=online&url=https%3A%2F%2Fz17.ade25.de)

Buildout installing the necessary tools to run a webserver on a specific domU.
Just boostrap the buildout and run

## Installation

This buildout is intended to be used via the development profile to provide
a ready to work on setup.

### Note:

In order to make this work locally you need to take a view extra steps. Please
refer to the [setup local directory documentation](docs/setup.md)

To get started with a new development environment
clone the buildout to your local machine and initialize the buildout:

``` bash
$ git clone git@github.com:username/z17.git
$ cd ./z17
$ b5 install
```

We use the globally installed task runner `b5` for the project. The buildout is intended to be used with a docker setup that mirrors the production environment. Therefore the build requires a local docker and traefik installation.


## Provided services:

* Nginx (Port 80)
* Varnish (Port 8100)
* haproxy (Port 8200)
* runscript
* logrotation
* supervisord (controlling the isntalled zope instances)


## Usage

Refer to [usage documentation](docs/usage.md)

