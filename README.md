# NAME

docker-control - Docker Control Script for MacOS and Linux

# VERSION

Version 0.0.1

# LICENCE AND COPYRIGHT

Copyright (c) 2019 Matthias Nott (mnott (at) mnsoft.org).

Licensed under WTFPL.


# INTRODUCTION

            This is a little script to help you control your
            docker environments.

# SYNOPSIS

I am completely unwilling to keep typing long commands to control
my docker containers and images. Hence I've created docker-control.

# Installation

Just put the "d" script somewhere into your path.

# Configuration

There is really only one thing to configure - the editor at the
top of the script. I am using Sublime Text, for which I've a
shortcut "e", but in general, something like "vi" should be good
for you here. It is only ever used when you want to edit the
Dockerfile right from the menu.

# Use

If you run "d" from within a location where you have a Dockerfile
or a docker-compose.yaml, you'll be able to also execute a build.
I basically only use docker-compose, even if I have only one single
container - the yaml file is, for me, a much easier way to define
all my runtime settings.

Note that the "up" and "down" commands only appear if you are in
a directory that contains a docker-compose.yaml. Note also that
"down" is actually a "stop" since quite often I am experimenting
with the content of a docker container before I decide what I want
to move into the docker file. docker-compose down will remove the
container, which I don't want it to do.

