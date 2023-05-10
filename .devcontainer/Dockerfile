FROM mcr.microsoft.com/devcontainers/cpp:0-ubuntu-22.04

#ARG REINSTALL_CMAKE_VERSION_FROM_SOURCE="3.22.2"

#COPY ./reinstall-cmake.sh /tmp/

#RUN if [ "${REINSTALL_CMAKE_VERSION_FROM_SOURCE}" != "none" ]; then \
#    chmod +x /tmp/reinstall-cmake.sh && /tmp/reinstall-cmake.sh ${REINSTALL_CMAKE_VERSION_FROM_SOURCE}; \
#    fi \
#    && rm -f /tmp/reinstall-cmake.sh

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends clang-14 clangd-14 libaio1 libaio-dev \
    && sudo ln -s /usr/bin/clangd-14 /usr/bin/clangd
