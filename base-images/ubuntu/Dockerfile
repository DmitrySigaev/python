# На всякий случай напоминаю, что Dockerfile всегда должен начинаться с импорта базового образа.
# Для этого используется ключевое слово 'FROM'.
# Здесь нам нужно импортировать образ python (с DockerHub).
# В результате мы, в качестве имени образа, указываем 'python', а в качестве версии - 'latest'.

FROM ubuntu:latest
ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get install -y --no-install-recommends zip unzip git build-essential  ca-certificates \
     python3-dev cmake make curl tar software-properties-common qtbase5-dev libgsl-dev  libgtest-dev libboost-all-dev


RUN add-apt-repository ppa:ubuntu-toolchain-r/test -y  && \
      apt-get update -y && \
      apt-get install g++-9 -y


#RUN cd /opt && git clone https://github.com/microsoft/vcpkg.git vcpkg
#RUN cd /opt/vcpkg && ls .
#RUN cd /opt/vcpkg && ./bootstrap-vcpkg.sh

#RUN cd /opt/vcpkg && ./vcpkg install boost-python:x64-linux
#RUN cd /opt/vcpkg && ./vcpkg install gsl:x64-linux
#RUN cd /opt/vcpkg && ./vcpkg install gtest:x64-linux
#RUN cd /opt/vcpkg && ./vcpkg install qt5[core]:x64-linux

