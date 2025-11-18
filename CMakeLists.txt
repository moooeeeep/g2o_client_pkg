cmake_minimum_required(VERSION 3.1)

project(g2o_client_pkg VERSION "3.0.0")

find_package(g2o REQUIRED)

add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME}
  g2o::core
)

