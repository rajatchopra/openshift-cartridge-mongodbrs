# OpenShift MongoDB Cartridge for Replica Sets

Use this downloadable cartridge to get mongo replica set with 3 gears.
rhc cartridge add https://raw.github.com/rajatchopra/openshift-cartridge-mongodbrs/master/metadata/manifest.yml --app <appname>

Be sure that your setup allows gears with atleast 2G of disk space per gear or this cartridge will fail.
