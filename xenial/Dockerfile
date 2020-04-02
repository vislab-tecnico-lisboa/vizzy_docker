# This is an auto generated Dockerfile for ros:ros-core
# generated from docker_images/create_ros_core_image.Dockerfile.em
FROM ubuntu:xenial

# install packages
RUN apt-get update && apt-get install -q -y \
    dirmngr \
    gnupg2 \
    lsb-release \
    add-apt-key \
    git \
    sudo \
    && rm -rf /var/lib/apt/lists/*


# setup environment
ENV LANG C.UTF-8
ENV LC_ALL C.UTF-8

# create Vizzy user
RUN adduser --disabled-password --gecos '' vizzy
# add sudo capabilities
RUN usermod -aG sudo vizzy

