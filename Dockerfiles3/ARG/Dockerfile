ARG VERSION
#FROM almalinux:${VERSION}
# docker build -t arg:v1 --build-arg VERSION=8 .    --> To create the image by providing version at runtime.
FROM almalinux:${VERSION:-8}   
# The above syntax is to set the default version if any version is not provided at runtime.
ARG GREETING
# ARG GREETING="hi good morning"
RUN echo "$GREETING"
RUN echo "$VERSION"
# docker build -t arg:v1 --build-arg VERSION=9 --build-arg GREETING=hello .
ENV GREET=${GREETING}