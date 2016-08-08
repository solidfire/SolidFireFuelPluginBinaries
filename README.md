# SolidFireFuelPluginBinaries
This repo contains the SolidFire Fuel Plugin binaries and checksums.

Binaries for the releases prior to Fuel 8.0 may be found in the
[Mirantis Plugin Catalog](https://www.mirantis.com/validated-solution-integrations/fuel-plugins/)

## Simple install instructions

#### Copy the plugin to an already installed Fuel Master node.
   If you do not have the Fuel Master node yet, follow the instructions from the
   official OpenStack Fuel documentation.

   Once you have the Fuel master node installed copy the rpm to the fuel
   master node:

      # scp cinder_solidfire-3.0-3.0.0-1.noarch.rpm \
          root@:<the_Fuel_Master_node_IP>:/tmp

#### Log into the Fuel Master node and install the plugin:

        # cd /tmp
        # fuel plugins --install /tmp/cinder_solidfire-3.0-3.0.0-1.noarch.rpm
        ...
        # fuel plugins list
        id | name             | version | package_version | releases
        ---+------------------+---------+-----------------+--------------------
        1  | cinder_netapp    | 5.0.0   | 4.0.0           | ubuntu (mitaka-9.0)

