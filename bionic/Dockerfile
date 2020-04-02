# This is an auto generated Dockerfile for ros:ros-core
# generated from docker_images/create_ros_core_image.Dockerfile.em
FROM ubuntu:bionic

# install packages
RUN apt-get update && apt-get install -q -y \
    dirmngr \
    gnupg2 \
    lsb-release \
    add-apt-key \
    git \
    sudo \
    && rm -rf /var/lib/apt/lists/*

# setup keys
#RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

# setup sources.list
#RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
RUN apt update -y
#ENV DEBIAN_FRONTEND=noninteractive
#RUN apt-get install -y tzdata
#ENV ROS_DISTRO melodic

# setup environment
ENV LANG C.UTF-8
ENV LC_ALL C.UTF-8

# create Vizzy user
RUN adduser --disabled-password --gecos '' vizzy
# add sudo capabilities
RUN usermod -aG sudo vizzy

