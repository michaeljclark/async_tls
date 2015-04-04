# async TLS test

a simple (and currently buggy) example of asynchronous TLS

Read TODO comment in `openssl_async_echo_server.cc` regarding SSL_do_handshake bug

## Overview
  * very simple example of non-blocking TLS
  * tested with boringssl and openssl
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
  * in second terminal (run twice to trigger bug)
````
./bin/openssl_async_echo_client
````
