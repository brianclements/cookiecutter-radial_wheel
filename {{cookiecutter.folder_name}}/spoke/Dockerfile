# Spoke Dockerfile for {{cookiecutter.wheel_name}}

FROM            radial/spoke-base:latest
MAINTAINER      Brian Clements <radial@brianclements.net>

# Install packages
ENV             DEBIAN_FRONTEND noninteractive
RUN             apt-get -q update && apt-get -qyV install \
                    {{NULL}} &&\
                apt-get clean

# Configure Spoke settings
ENV             SPOKE_NAME {{cookiecutter.wheel_name}}
ENV             SPOKE_CMD {{cookiecutter.wheel_name}}

COPY            /entrypoint.sh /entrypoint.sh
