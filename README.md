# Asynchronous TLS test

a simple example of asynchronous TLS

## Overview
  * very simple example of non-blocking TLS
  * compiles with boringssl and openssl
  * needs testing and feedback
  * probably leaks

## Compiling
````
clang++ -std=c++11 openssl_async_echo_client.cc -lcrypto -lssl -o openssl_async_echo_client
clang++ -std=c++11 openssl_async_echo_server.cc -lcrypto -lssl -o openssl_async_echo_server
````

## Running
  * in first terminal
````
./bin/openssl_async_echo_server
````
  * in second terminal
````
./bin/openssl_async_echo_client
````
