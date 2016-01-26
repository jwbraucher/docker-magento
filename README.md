# braucher/magento 1.0.1

This [braucher/magento](https://hub.docker.com/r/braucher/magento/) docker image provides an Ubuntu 14.04 magento application container.

The [braucher/magento](https://hub.docker.com/r/braucher/magento/) image also includes the following:

* mage
* postfix
* /app entrypoint

## Usage

By default, ```/app start``` is the entrypoint and command, 
the daemon listens on port 9000, and files are served from /var/www/app.
Run ```/app install``` to install Magento
Run ```/app backup``` to backup the Magento installation

See the
[docker-compose.yml from the sample-project branch](https://github.com/jwbraucher/docker-magento/tree/latest/docker-compose.yml)
for an example of how to build a new project from this image using the
following Docker images:

* [braucher/magento](https://hub.docker.com/r/braucher/magento/) (this one)
* [braucher/fcgi](https://hub.docker.com/r/braucher/fcgi/)
* [mysql](https://hub.docker.com/r/_/mysql/)

To start your own image, fork this project and modify the following files:
* Makefile.local
* docker-compose.yml
* app/app.*

### Environment Variables

See the [/app.env script](https://github.com/jwbraucher/docker-magento/tree/latest/app/app.env)
for all accepted parameters. 

## Development
See DEVELOPMENT.md

## License
MIT license

