# coretemp

## To build the driver yourself, go on your docker host and use follwing shell commands to build it.

mkdir driver-coretemp

cd driver-coretemp

git clone https://github.com/xcp-ng/xcp-ng-build-env

git clone https://github.com/rushikeshjadhav/coretemp.git

chown 1000 ./coretemp/ -R

./xcp-ng-build-env/run.py -b 8.0 --build-local coretemp/ --rm
