# Spoke Dockerfile for {{cookiecutter.wheel_name}}

FROM            radial/spoke-base:latest
MAINTAINER      Brian Clements <radial@brianclements.net>

# Install packages
ENV             DEBIAN_FRONTEND noninteractive
RUN             apt-get -q update && apt-get -qyV install \
                    {{NULL}} &&\
                apt-get clean
RUN             env --unset=DEBIAN_FRONTEND

# File Permissions
ENV             SPOKE_NAME {{cookiecutter.wheel_name}}

# Public keys
ENV             GH_USER {{cookiecutter.github_username}}
