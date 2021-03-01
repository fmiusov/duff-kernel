# Installation

## First spin up a docker container - 

$ docker build buildenv -t duffkernel-buildenv

__Linux or MacOS:__  docker run --rm -it -v $pwd:/root/env duffkernel-buildenv

__Windows:__         docker run --rm -it -v %cd%:/root/env duffkernel-buildenv

__Boot into qemu__
qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso

## Troubleshooting

1. sudo or admin access may be needed to run the above command depending on your docker preferences
2. docker is not running
3. qemu file path is not added in environment variables

