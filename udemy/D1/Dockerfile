# Fundamentals
ARG CODE_VERSION=16.04
FROM ubuntu:${CODE_VERSION}

# Configuration
RUN apt-get update && apt-get install -y curl \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir home/codes

# username
ENV USER vpb-canvas
# shell to use
ENV SHELL /bin/bash
# logname to appear?
ENV LOGNAME vpb-canv

# Execution

# opens bash to type?
# get image ready to run
CMD ["bash"]

