# SolidFireFuelPluginBinaries
This repo contains the SolidFire Fuel Plugin binaries and checksums.

Binaries for the releases prior to this release may be found in the
[Mirantis Plugin Catalog](https://www.mirantis.com/validated-solution-integrations/fuel-plugins/)

## Simple install instructions

#### Copy the plugin to an already installed Fuel Master node.
   If you do not have the Fuel Master node yet, follow the instructions from the
   official OpenStack Fuel documentation:

       # scp fuel-plugin-solidfire-cinder-2.0-2.0.0-1.noarch.rpm \
        root@:<the_Fuel_Master_node_IP>:/tmp

#### Log into the Fuel Master node and install the plugin:

        # cd /tmp
        # fuel plugins --install /tmp/fuel-plugin-solidfire-cinder-2.0-2.0.0-1.noarch.rpm
        ...
        # fuel plugins list
        id | name                         | version | package_version
        ---|------------------------------|---------|----------------
        1  | fuel-plugin-solidfire-cinder | 2.0.0   | 4.0.0
