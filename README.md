# centreon-install


Centreon autoinstall for Debian (with centreon-engine)

Tested on Debian Wheezy with PHP 5.3

## Default install
### Version and URLs
- CLIB_VER="1.2.0"
- CONNECTOR_VER="1.0.2"
- ENGINE_VER="1.4.6"
- PLUGIN_VER="2.0.3"
- BROKER_VER="2.6.3"
- CENTREON_VER="2.5.2"
- CLAPI_VER="1.6.1"

## Temp and install directories

- DL_DIR="/usr/local/src"
- INSTALL_DIR="/usr/local"

## Users, groups and passwords

- MYSQL_PASSWORD="password"
- ENGINE_USER="centreon-engine"
- ENGINE_GROUP="centreon-engine"
- BROKER_USER="centreon-broker"
- BROKER_GROUP="centreon-broker"
- CENTREON_USER="centreon"
- CENTREON_GROUP="centreon"

## Usage

 Change your vars at the beginning of the script

        sudo ./centreon.sh

        http://localhost/centreon/

## Complete the web install

        Monitoring engine                        => centreon-engine
        Centreon Engine directory                => /usr/local/centreon-engine
        Centreon Engine Stats binary             => /usr/local/centreon-engine/bin/centenginestats
        Centreon Engine var lib directory        => /var/lib/centreon-engine
        Centreon Engine Connector path           => /usr/local/centreon-connector
        Centreon Engine Library (*.so) directory => /usr/local/centreon-engine/lib/centreon-engine/
        Embedded Perl initialisation file        =>

## Broker Module Information

        Broker Module                            => centreon-broker
        Centreon Broker etc directory            => /usr/local/centreon-broker/etc
        Centreon Broker module (cbmod.so)        => /usr/local/centreon-broker/lib/cbmod.so
        Centreon Broker log directory            => /var/log/centreon-broker/
        Retention file directory                 => /var/lib/centreon-broker
        Centreon Broker lib (*.so) directory     => /usr/local/centreon-broker/lib/centreon-broker/

## Complete the web wizard

## Restart cbd
        service cbd restart

# Roadmap

- installing Centreon 2.x on Debian Wheezy with PHP 5.4 (the standard version)
