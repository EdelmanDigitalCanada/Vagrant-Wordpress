# Vagruntpress  

![Wordpress](http://www.takgraph.ir/wp-content/uploads/2014/01/wordpress-logo-notext-rgb3.png)
![Vagrant](http://www.layh.com/wp-content/uploads/2014/05/logo_vagrant.png)
![Grunt](http://i.imgur.com/gzPamBO.png)

https://wordpress.org/  
https://www.vagrantup.com/  
http://gruntjs.com/  


### Prerequisite

* [Virtual Box] - The Virtual Machine Manager
* [Vagrant] - Development environments based on VM
* [VagrantHostManager] - Vagrant Plugin to automatically update your local hosts file
* [VagrantExec] - Vagrant plugin to allow direct command line execution from the host machine
* [Grunt] - Javascript Task Runner  

### Specifications

Wordpress installation includes:
* [WPCLI] - Command line support for Wordpress
* [WpSyncDB] - A plugin that helps you to sync your databases between environments
* [WpSyncDBMedia] - A addon to sync your medias between environments
* [WpSyncDBCli] - An another addon to handle migrations from the command line

### Configuration

You can modify the configuration in 'config.yaml'

### What it does?

The simple command `vagrant up` will generate a Wordpress installation ready to be used.

### Main Commands

From the project root

| Command                              |      Action                                               |
|--------------------------------------|:---------------------------------------------------------:|
| vagrant up                           |  start the vagrant machine                                |
| vagrant reload --provision           |  restart the vagrant machine                              |
| vagrant halt                         |  stop the vagrant machine                                 |
| vagrant exec wp wpsdb migrate 1      |  run WP Sync DB profile #1 (sync dev with local)          |

From the project theme folder

| Command                              |      Action                                               |
|--------------------------------------|:---------------------------------------------------------:|
| grunt watch                          |  start the grunt watcher (for scss and js changes)        |

[Virtual Box]:https://www.virtualbox.org/
[Vagrant]:https://www.vagrantup.com/
[VagrantHostManager]:https://github.com/michaelbontyes/vagrant-hostmanager
[VagrantExec]:https://github.com/michaelbontyes/vagrant-exec
[Grunt]:http://gruntjs.com/

[WPCLI]:http://wp-cli.org/
[WpSyncDB]:https://github.com/wp-sync-db/wp-sync-db
[WpSyncDBMedia]:https://github.com/wp-sync-db/wp-sync-db-media-files
[WpSyncDBCli]:https://github.com/wp-sync-db/wp-sync-db-cli
