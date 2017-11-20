# cmplopes/alpine-gfortran
Docker GNU Fortran over Alpine Linux

## 
```
$ docker pull -t cmplopes/alpine-gfortran:[TAG]
```

## Suported Tags

6.4, latest (over alpine:edge)

6.3 (over alpine:3.6)

6.2 (over alpine:3.5)

5.3 (over alpine:3.4)


## Check GNU Fortran version
```
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3
```
or
```
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3 gfortran --version
```

## Compile, link and run a Fortran program
```
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3 gfortran -Wall -o test /source/test.f90
$ docker run --rm -it -v $(pwd):/source cmplopes/alpine:gfortran:6.3 ./test
```
