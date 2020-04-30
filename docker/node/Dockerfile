FROM ubuntu:latest

RUN apt update
RUN apt install -y dos2unix

# Move scripts
WORKDIR /srv
ADD ./scripts /srv/scripts
RUN chmod +x /srv/scripts -R
RUN find /srv/scripts -type f -print0 | xargs -0 dos2unix --

# Setup Image
RUN ./scripts/install/misc

# Setup Environment


# Setup APP


# Run Sevices
