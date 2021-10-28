cmake_minimum_required(VERSION 3.12)

project(xi)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(openssl_async_echo_client src/openssl_async_echo_client.cc)
target_link_libraries(openssl_async_echo_client crypto ssl)

add_executable(openssl_async_echo_server src/openssl_async_echo_server.cc)
target_link_libraries(openssl_async_echo_server crypto ssl)
