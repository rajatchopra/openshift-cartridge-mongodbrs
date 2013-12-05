# OpenShift MongoDB Cartridge for Replica Sets

Use this downloadable cartridge to get mongo replica set with 3 gears. Note that this is a work in progress.

rhc cartridge add https://raw.github.com/rajatchopra/openshift-cartridge-mongodbrs/master/metadata/manifest.yml --app your_apps_name

Things to keep in mind -

a. Be sure that your setup allows gears with atleast 2G of disk space per gear or this cartridge will fail. 
     Quick fix on a sample setup - edit /etc/openshift/resource_limits.conf on all nodes and set quota_blocks=2097152, then reboot.

b. There is no auth present in this setup (yet).

c. The usual way of connecting to mongo replica setup will change also. Current method of using $OPENSHIFT_MONGODB_DB_HOST:$OPENSHIFT_MONGODB_DB_PORT will not work smoothly because now there are secondary endpoints too.


