# PHPUnit Docker Container

[![Docker pull](https://img.shields.io/docker/pulls/phpunit/phpunit.svg)](https://hub.docker.com/r/phpunit/phpunit/) [![Docker pull](https://img.shields.io/docker/stars/phpunit/phpunit.svg)](https://hub.docker.com/r/phpunit/phpunit/) [![Github issues](https://img.shields.io/github/issues/JulienBreux/phpunit-docker.svg)](https://github.com/JulienBreux/phpunit-docker/issues) [![License](https://img.shields.io/github/license/JulienBreux/phpunit-docker.svg)](https://github.com/JulienBreux/phpunit-docker/blob/master/LICENSE)


[Docker](https://www.docker.com) container to install and run [PHPUnit](https://phpunit.de/).

## Features

* [PHPUnit](https://www.phpunit.de/)
  * Latest snapshot (master)
  * [`5.0.3`](https://github.com/sebastianbergmann/phpunit/blob/5.0/ChangeLog-5.0.md#503---2015-10-02)
  * [`4.8.5`](https://github.com/sebastianbergmann/phpunit/blob/4.8/ChangeLog-4.8.md#485---2015-08-19)
  * [`4.8.4`](https://github.com/sebastianbergmann/phpunit/blob/4.8/ChangeLog-4.8.md#484---2015-08-15)
  * [`4.8.3`](https://github.com/sebastianbergmann/phpunit/blob/4.8/ChangeLog-4.8.md#483---2015-08-10)
  * [`4.7.7`](https://github.com/sebastianbergmann/phpunit/blob/4.7/ChangeLog-4.7.md#477---2015-07-13)
  * [`4.6.10`](https://github.com/sebastianbergmann/phpunit/blob/4.6/ChangeLog-4.6.md#phpunit-4610)
  * [`4.6.6`](https://github.com/sebastianbergmann/phpunit/blob/4.6/ChangeLog-4.6.md#phpunit-466)
* [PHP](https://php.net) [5.6](https://php.net/ChangeLog-5.php)
* [Xdebug](https://xdebug.org/) [2.3.3](https://xdebug.org/updates.php#x_2_3_3)

## Installation / Usage

1. Install the phpunit/phpunit container:

    ``` sh
	$ docker pull phpunit/phpunit
	```

2. Create a phpunit.xml defining your tests suites.

    ``` xml
...
    ```

3. Run PHPUnit through the PHPUnit container:

    ``` sh
	$ docker run -v $(pwd):/app phpunit/phpunit run
    ```

To run, test and develop the PHPUnit Dockerfile itself, you must use the source directly:

1. Download the source:

    ``` sh
	$ git clone https://github.com/JulienBreux/phpunit-docker.git
    ```

2. Switch to the phpunit-docker directory:

    ``` sh
	$ cd phpunit-docker
    ```

3. Build the container:

    ``` sh
	$ docker build -t phpunit/phpunit .
    ```

4. Test running the container:

    ``` sh
	$ docker run phpunit/phpunit --help
	```
