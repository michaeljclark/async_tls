cmake_minimum_required(VERSION 3.12)

project(xi)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(async_tls_echo_client src/async_tls_echo_client.cc)
target_link_libraries(async_tls_echo_client crypto ssl)

add_executable(async_tls_echo_server src/async_tls_echo_server.cc)
target_link_libraries(async_tls_echo_server crypto ssl)
