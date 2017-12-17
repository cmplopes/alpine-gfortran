FROM alpine:3.7
MAINTAINER Carlos Lopes "cmplopes67@gmail.com"

RUN apk add --no-cache bash bash-doc bash-completion
RUN apk add --no-cache musl-dev 
RUN apk add --no-cache gfortran

WORKDIR /source

CMD gfortran --version
