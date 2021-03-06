#Vagrant Phalcon Box setup

A slight modification of https://github.com/web-solution/vagrant-symfony2-box to work with phalcon

* Using Mysql 5.6 version
* added elasticsearch
* added beanstalkd
* mongodb removed
* capifony removed
* phalcon.ini is in the /puppet/files/phalcon.ini
* Config params is in the ```/puppet/manifests/core/params.pp```. Change this values spesifi to your needs.

* Vagrant automatically setups database with this setup:

    * Username: root
    * Password: core::params::dbroot_password
    * Database: core::params::dbname


## Requirements
* [VirtualBox](https://www.virtualbox.org)
* [Vagrant](http://vagrantup.com)
* [vagrant-hostmanager](https://github.com/smdahlen/vagrant-hostmanager)
	* `vagrant plugin install vagrant-hostmanager`

## Installation
####This setup is based and tested with Ubuntu Precise 64 bit base box, with Vagrant 1.5.1 version

Clone this repository

    ```$ git clone https://github.com/jeffreycahyono/vagrant-phalcon-box.git```

* run vagrant (for the first time it should take up to 30-60 min)
    ```$ vagrant up```

* Web server is accessible with http://www.phalcon-box.local (Host address can be changed in Vagrantfile)

* PhpMyAdmin is accessible with http://www.phalcon-box.local/phpmyadmin


## Installed components

* [Nginx](http://nginx.org/en/)
* [MySQL](http://www.mysql.com/)
* [PHP-FPM](http://php-fpm.org/)
* [PhpMyAdmin](http://www.phpmyadmin.net/home_page/index.php)
* [MongoDB](http://www.mongodb.org/)
* [Redis](http://redis.io/)
* [GiT](http://git-scm.com/)
* [Composer](http://getcomposer.org)
* [Vim](http://www.vim.org/)
* [PEAR](http://pear.php.net/)
* [cURL](http://curl.haxx.se/)
* [Node.js](http://nodejs.org/)
* [npm](https://npmjs.org/)
* [less](http://lesscss.org/)
* [OpenJDK](http://openjdk.java.net/)
* [sass](http://sass-lang.com/)
* [Compass](http://compass-style.org/)
* [Imagic](http://www.imagemagick.org/script/index.php)
* [Capistrano](https://github.com/capistrano/capistrano)
* [Capifony](http://capifony.org/) --removed--
* [phpqatools](http://phpqatools.org/)
* [memcached](http://memcached.org/)
