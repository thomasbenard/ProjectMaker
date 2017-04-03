cmake_minimum_required(VERSION 3.6)

set(PROJECT_NAME TemplateProject)
project(TemplateProject)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=gnu++11")

set(SOURCE_FILES main.cpp )
add_executable(run_TemplateProject ${SOURCE_FILES})

add_subdirectory(unit_tests)
add_subdirectory(src)

target_link_libraries(run_TemplateProject TemplateProject_src)