# waypoint-spk

This package is heavily based from the work done for [gogs-spk](https://github.com/alexandregz/gogs-spk)

[waypoint](https://waypointproject.io) (Secret storage) SPK package ([Synology PacKages](https://www.synology.com/en-us/dsm/app_packages))

Install waypoint into a Synology NAS.

## Requirements

Only tested on x64 (DS916+) could work on ARM since a waypoint binary exists.

## Usage

Change **Package Center -> Trust Level** to **Any Publisher** and import manually the package from **Manual install**.
Finally, install with waypoint web installation.

## Configuration

You can store your configuration using a `conf.d` folder inside `1_create_package/waypoint/`. If you don't want to ship your configurations with the package, you can use `/etc/waypoint`.

## To use with another arch

Download the binary from https://www.waypointproject.io/downloads.html, replace the content from **1_create_package/waypoint** directory and exec create_spk.sh:

```~/src/waypoint-spk(master)$ rm -rf 1_create_package/waypoint/ && unzip waypoint_1.1.2.zip && mv waypoint ./1_create_package/```

```$ sh create_spk.sh```

