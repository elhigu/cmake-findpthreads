Cross platform  FindPthreads.cmake
==================================

Finds out if pthreads is available and suggests how to get it for your platform.
(e.g. download binary distribution for Windows and setup PTHREADS_ROOT env variable)

For Windows macro tries to find precompiled pthread libs which can be downloaded from 
https://sourceware.org/pthreads-win32/

## Try it out

```
git clone https://github.com/elhigu/cmake-findpthreads.git
mkdir build
cd build
cmake ../cmake-findpthreads
```

In Windows you would probably use Visual Studio:

1. Download binary package for Windows from https://sourceware.org/pthreads-win32/
2. Setup your PTHREADS_ROOT environment variable to where your library is

```
cmake -G "Visual Studio 12" ../cmake-findpthreads
cmake -G "Visual Studio 12 Win64" ../cmake-findpthreads
```

