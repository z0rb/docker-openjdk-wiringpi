![Docker Build Status](https://img.shields.io/docker/build/z0rb/openjdk-wiringpi.svg?style=for-the-badge)

# z0rb/openjdk-wiringpi
arm32v7 OpenJDK docker image extended with WiringPi.

The current image is restricted to arm32v7 beause of the following bug in docker upstream: https://github.com/moby/moby/issues/34875
Once the bug is resolved the image can be adapted for multiple arm variants.

# Build Locally

In order to build the image locally on any architecture you will need to install qemu and register it with the build agent. The static binary should be copied to the `hooks` directory.
The required steps are summarized in the [docker hub post checkout script](hooks/post_checkout). This script runs apt-get so it will require root privileges, check the script first before executing:

`sudo ./hooks/post_checkout`
