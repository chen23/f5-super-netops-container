############################################################
# Dockerfile to build f5-super-netops enablement container
# Based on Alpine Linux, seasoned with tools and workflows
############################################################

# Start with an awesome, tiny Linux distro.
FROM f5devcentral/f5-super-netops-container:base

LABEL maintainer "eric.chen@f5.com"

# Set the SNOPS image name
ENV SNOPS_IMAGE f5-cccl

# Copy in base FS from repo
COPY fs /

#Add libraries to compile ansible
RUN apk add --update gcc python2-dev linux-headers libc-dev libffi libffi-dev openssl openssl-dev

#install f5-cccl
#RUN pip install ansible bigsuds f5-sdk netaddr deepdiff ansible-lint ansible-review
