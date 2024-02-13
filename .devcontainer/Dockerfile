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

#install ZSH
RUN apt install zsh -y

#install curl
RUN apt install curl -y

# install nodejs
RUN apt install nodejs -y
RUN apt install npm -y

# readline lib
RUN apt-get install -y libreadline-dev

#install paco
RUN bash -c "$(curl -fsSL https://raw.github.com/xicodomingues/francinette/master/bin/install.sh)"

# Install python and norminette
RUN apt install python3-pip -y
RUN apt-get install python-dev-is-python3 -y
RUN apt install python3.10-venv -y
RUN python3 -m pip install --upgrade pip setuptools
RUN python3 -m pip install norminette

CMD [ "zsh" ]
