Affordable AUV Platform
=======================

Affordable AUV Platform **Beaglebone** buildconf


## Installation Instruction

Confirm the ruby version using the command below:

```bash
$ ruby --version
```

The current rock version requires the ruby version equal or higher than 2.0.
Before continue the installation is needed to install the correctly ruby version.

## Create sytem folder

In the beaglebone, create the folder used to store the Rock Robotics packages, such as shown below:

```bash
$ mkdir -p ~/auv_platform/dev
```

## Download the autoproj_bootstrap

Go into the folder created previously and download the autoproj_bootstrap.

```
$ cd ~/auv_platform/dev
```

The **autoproj_bootstrap** contains the instructions to install the **package_set** required by beaglebone.

```bash
$ wget http://www.rock-robotics.org/master/autoproj_bootstrap
```

## Bootstrap the beaglebone buildconf

Execute the command below to download and configure the **package set** used in the beaglebone

```bash
$ ruby2.0 autoproj_bootstrap git git@github.com:affordable-auv-platform/beaglebone-buildconf.git
```

## Set the environment

Execute the command `. .env.sh` to set up the environment.


## Update the system

Execute the command `aup` to checkout and update the packages.

## Compiling the system

Execute the command `amake` to compile the packages.
