# Asynchronous TLS

a very simple example of asynchronous TLS using OpenSSL.

## Building

requires cmake and openssl.

````
cmake -G Ninja -B build
cmake --build build -- --verbose
````

## Running

in first terminal
````
./build/async_tls_echo_server
````

in second terminal
````
./build/async_tls_echo_client
````
