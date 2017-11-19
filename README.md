# alpine-gfortran
Docker GNU Fortran over Alpine Linux

## 
```
$ docker pull -t cmplopes/alpine-gfortran:[TAG]
```

## Check version
```
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3
```
or
```
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3 gfortran --version
```

## Compile, link and run Fortran program
```
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3 gfortran -Wall -o test /source/test.f90
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3 ./test
```
