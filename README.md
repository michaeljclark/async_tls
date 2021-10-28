# Asynchronous TLS

a very simple example of asynchronous TLS using OpenSSL.

## Building

requires cmake and openssl.

````
cmake -G Ninja -B build
cmake --build build -- --verbose
````

## Running
  * in first terminal
````
./build/openssl_async_echo_server
````
  * in second terminal
````
./build/openssl_async_echo_client
````
