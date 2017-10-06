## OkHttp fork for C++ 
[![Build Status](https://travis-ci.org/Good-Pudge/okhttp-fork.svg?branch=master)](https://travis-ci.org/Good-Pudge/okhttp-fork)
[![Build status](https://ci.appveyor.com/api/projects/status/sfpb0w34urnfn59l?svg=true)](https://ci.appveyor.com/project/Good-Pudge/okhttp-fork)
#### Required libraries:
* [OpenSSL](https://github.com/openssl/openssl)

#### Installation:
First step:
````bash
git clone https://github.com/Good-Pudge/OkHttpFork.git
cd OkHttpFork
cmake .
````
Second step for different systems:
* ##### Windows:
    * MSVC:
    ````bash
    cmake --build . --target INSTALL --config Release
    ````
    * MinGW:
    ````bash
    mingw32-make -j2
    mingw32-make install
    ````
* ##### UNIX-like:
    ````bash
    make -j2
    sudo make install
    ````

#### Implemented components:
* Headers
* HttpURL
* MediaType
* RequestBody
* ResponseBody
* Socket (Windows, POSIX for now)
* SSLSocket (Windows, POSIX for now)
* Cookie
* CookieJar
* Call
* DNS
* CacheControl
