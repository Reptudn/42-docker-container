FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN apt-get update && apt-get install -y xz-utils

# Install gcc
RUN apt-get install gcc -y

# Install clang
RUN apt-get install clang -y

# Install git
RUN apt install git-all -y

# Install valgrind
RUN apt-get install git-core sudo build-essential cmake valgrind libcppunit-dev -y

# Install python and norminette
RUN apt install python3-pip -y
RUN python3 -m pip install --upgrade pip setuptools
RUN python3 -m pip install norminette