FROM alpine:3.12
LABEL maintainer="Carlos Lopes (cmplopes67@gmail.com)"

RUN apk add --no-cache bash bash-doc bash-completion
RUN apk add --no-cache musl-dev 
RUN apk add --no-cache gfortran gdb make

WORKDIR /source

CMD gfortran --version
