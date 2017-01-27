# quemu-on-arm

Automatic build on docker-hub: https://hub.docker.com/r/awalach/armhf-ubuntu/

##How to use
On ubuntu (x86_64):

install:
    
    apt-get install qemu-user-static

run:

    docker run -it --rm awalach/armhf-ubuntu:latest

test:

    uname -a
    Linux 16ace0eb37c9 4.4.0-59-generic #80-Ubuntu SMP Fri Jan 6 17:47:47 UTC 2017 armv7l armv7l armv7l GNU/Linux

Or even simpler, using base "ioft/armhf-ubuntu:16.10" image

    docker run -it --rm -v /usr/bin/qemu-arm-static:/usr/bin/qemu-arm-static ioft/armhf-ubuntu:16.10

