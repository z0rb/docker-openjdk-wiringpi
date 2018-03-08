![Docker Build Status](https://img.shields.io/docker/build/z0rb/openjdk-wiringpi.svg?style=for-the-badge)

# docker-openjdk-wiringpi
arm32v7 OpenJDK docker image extended with WiringPi.

The current image is restricted to arm32v7 beause of the following bug in docker upstream: https://github.com/moby/moby/issues/34875
Once the bug is resolved the image can be adapted for multiple arm variants.
